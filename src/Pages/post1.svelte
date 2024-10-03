<script>
    import Artigo from "./artigo.svelte";
</script>

<Artigo id="post1">
    <div class="flex flex-col md:flex-row"> <!-- Flex em coluna por padrão, em linha a partir de telas médias -->
        <div class="flex-1 pr-4"> <!-- Bloco de texto à esquerda -->
            <h2>
                O valor e o preço do tempo
            </h2>
            <h3>02/10/2024 - Campo Largo</h3>
            <h3>Autor - Felipe</h3>
            <p>
                Imagine que você recebe R$ 61.200 todos os dias, mas precisa gastá-los até meia-noite, ou o dinheiro desaparece. Inicialmente, você aproveitará para comprar coisas bonitas, viajar e se divertir. No entanto, com o passar do tempo, essa rotina poderá se tornar maçante, levando a desperdícios.

                De forma semelhante, Deus nos presenteia com 86.400 segundos diariamente, esperando que façamos bom uso desse tempo. Mas quanto vale realmente nosso tempo? Se gastarmos cinco minutos treinando guitarra diariamente, em um ano teremos dedicado um dia inteiro a essa paixão. Por outro lado, se usarmos duas horas por dia em redes sociais, isso se transforma em quase um mês perdido em um ano.
            </p>
        </div>

        <div class="flex-1 pr-4"> <!-- Bloco de texto à direita -->
            <p>
                Nosso tempo é finito, e cada dia é uma oportunidade preciosa. Como nos ensina Mateus 6:27, não podemos acrescentar uma hora à nossa vida. O tempo é o recurso mais valioso que temos, e deve ser utilizado para nos aproximar de Deus e cumprir Sua obra. Investir tempo nas coisas de Deus fortalece nosso relacionamento com Ele e nos prepara para a eternidade.
                
                À medida que refletimos sobre a brevidade da vida, somos levados a valorizar cada momento. A morte, em vez de ser um motivo de temor, deve nos motivar a agir em relação à salvação dos que amamos.
                
                Eclesiastes 3 nos lembra que há um tempo para tudo, e devemos aproveitar a vida plenamente, mas sem esquecer da importância da pregação do evangelho. Portanto, aproximemo-nos de Deus, celebremos a vida e façamos bom uso do tempo, o recurso mais precioso que nos foi dado. O tempo urge, e cada segundo conta na construção de um legado que transcende esta vida.
            </p>
        </div>
    </div>

    <div class="image-container flex flex-col w-full mt-4"> <!-- Imagem abaixo dos blocos de texto -->
        <img src="src/public/tempo.jpg" alt="homem contemplando relógio" class="responsive-image">
    </div>
</Artigo>

