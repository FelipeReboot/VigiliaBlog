<script>
    import { openModal } from "../Store";
</script>

<header class="flex flex-col relative z-20">
    <div class="max-w-[1400px] bg-[#E8ECE4] mx-auto w-full flex items-center justify-between p-4 py-6 px-7">
        <a href="/">
            <h1 class="font-semibold text-5xl">VIGÍLIA</h1>
            <!-- "logo" -->
        </a>

        <!-- Botão de menu para telas pequenas -->
        <button
            on:click={() => ($openModal = true)}
            class="md:hidden lg:hidden grid place-items-center bg-[#E8ECE4]"
        >
            <i class="fa-solid fa-bars"></i>
        </button>

        <!-- Navegação principal -->
        <nav class="hidden md:flex items-center gap-4 lg:gap-6">
            <a
                href="https://ministerionovaalianca.vercel.app"
                target="_blank"
                class="duration-200 hover:text-indigo-400 cursor-pointer"
            >
                Nova Aliança
            </a>
            <a
                href="https://doemna.vercel.app/"
                target="_blank"
                class="duration-200 hover:text-indigo-400 cursor-pointer"
            >
                Contribua
            </a>
        </nav>
    </div>

    <!-- Linha cinza abaixo do cabeçalho -->
    <div class="h-0.5 bg-[#39393A] my-1 max-w-full"></div>
</header>

