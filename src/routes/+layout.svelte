<script>
  import "../app.css";
  import Footer from "../components/Footer.svelte";
  import { openModal } from "../Store";

  function reroute(href) {
    $openModal = false;
    window.location.href = href;
  }

  import { onMount } from 'svelte';

  onMount(() => {
      const closeModalOnEscape = (event) => {
          if (event.key === 'Escape') {
              $openModal = false;
          }
      };

      window.addEventListener('keydown', closeModalOnEscape);

      return () => {
          window.removeEventListener('keydown', closeModalOnEscape);
      };
  });
</script>

{#if $openModal}
  <div
    class="fixed top-0 left-0 w-screen h-screen
    bg-[#E8ECE4] z-50 flex flex-col gap-8 p-5 px-8 md:hidden"
    role="dialog"
    aria-labelledby="modal-title"
  >
    <div class="flex items-center justify-between gap-4 border-b pb-2">
      <a href="/">
        <h1 class="font-semibold text-5xl" id="modal-title">VIGÍLIA</h1>
      </a>
      <button
        on:click={() => ($openModal = false)}
        class="outline-none border-none"
      >
        <i class="fa-solid fa-xmark text-2xl"></i>
      </button>
    </div>
    <div class="flex flex-col gap-4">
      <button
        on:click={() => reroute('https://ministerionovaalianca.vercel.app')}
        class="bg-[#E8ECE4] border-none outline-none p-2 group duration-200 cursor-pointer text-left"
      >
        <p class="duration-200 group-hover:pl-2 poppins text-2xl font-semibold">
            Nova Aliança
            <i class="fa-solid fa-chevron-right text-lg pl-4"></i>
        </p>
      </button>

      <button
        on:click={() => reroute('https://doemna.vercel.app/')}
        class="bg-[#E8ECE4] border-none outline-none p-2 group duration-200 cursor-pointer text-left"
      >
        <p class="duration-200 group-hover:pl-2 poppins text-2xl font-semibold">
            Contribua
            <i class="fa-solid fa-chevron-right text-lg pl-4"></i>
        </p>
      </button>
    </div>
  </div>
{/if}

<slot />

