<script setup lang="ts">
import AtomTitle from '~/components/atoms/atomTitle/atomTitle.vue';
import AtomParagraph from '~/components/atoms/atomParagraph/paragraph.vue';
import {
    Carousel,
    CarouselContent,
    CarouselItem,
    CarouselNext,
    CarouselPrevious,
} from '@/components/ui/carousel'

const entregasSpy = [
    {
        id: 1,
        productName: 'Como Desenhar',
        thumb: "https://kronus.kebook.com.br/assets/8926ea06-fcf6-47c0-9c3a-440c1a3478a6/content-expert.png",
        archive: "1dpm-5fsVt0hRNwtjlBVHGJFkndZ_Jv3a",
        title: 'Desbloqueie o Artista: Técnicas e Práticas para Excelência em Desenho!',

        subtitle: 'Transforme suas ideias em arte: aprenda técnicas de desenho e pratique com experts! Torne-se um desenhista habilidoso e criativo.',

        aboutTitle: 'Aprenda a desenhar! Curso completo: técnicas básicas até avançadas, com muita prática. Transforme seu traço e expresse arte!',
        aboutProduct: 'Você já imaginou capturar o mundo com a ponta do seu lápis? Com o curso \"Artista Master em Desenho\", transformamos sua visão artística em realidade, levando você em uma jornada criativa incrível. Este curso é sua chave de ouro para descobrir os segredos do desenho, desde conceitos fundamentais até técnicas avançadas, acessíveis a todos os níveis de habilidade. Liberte o artista dentro de você!\n\nDesenvolvido por mestres da arte visual, nosso curso é um tesouro que oferece conteúdo prático e teórico, meticulosamente planejado para impulsionar sua habilidade e confiança. Exploramos perspectiva, sombreamento, composição e muito mais, tudo em um formato fácil de seguir. Veja seu progresso através de exercícios práticos que transformarão sua capacidade de desenhar em poucas semanas!\n\nNão deixe escapar a oportunidade de brilhar no mundo do desenho. A inscrição no \"Como Desenhar\" é uma decisão inteligente para quem deseja elevar sua arte. Espaços são limitados, então garanta seu lugar agora e comece a criar obras que capturam a essência da beleza ao seu redor. Vamos juntos desbloquear seu potencial ilimitado!',

        howTitle1: 'Técnicas Essenciais de Desenho',
        howDesc1: 'Explore os fundamentos do desenho e aprimore sua técnica com práticas efetivas em nosso curso completo.',

        howTitle2: 'Traços Precisos: Desenho',
        howDesc2: 'Explore técnicas essenciais de desenho com videoaulas detalhadas, guias práticos e feedback constante.',

        howTitle3: 'Desenho Master (não gostei desse aqui)',
        howDesc3: 'Aprimore suas habilidades artísticas aplicando técnicas essenciais e práticas direcionadas, aprendidas em nosso curso, para elevar seus desenhos a um novo patamar de excelência!',

        howTitle4: 'Desenho Prático',
        howDesc4: 'Descubra o universo do desenho! Aprenda conceitos fundamentais e pratique intensamente com nosso infoproduto inovador!',

        bonusTitle1: 'Guia Desmistificando Mitos',
        bonusDesc1: 'Descubra o que o mercado exige e quais caminhos seguir para se tornar um profissional.',
        bonusLil1Desc1: 'Compreenda as diferenças entre cursos e escolha o melhor para você.',
        bonusLil2Desc1: 'Descubra o que realmente importa para o mercado de trabalho.',
        bonusLil3Desc1: 'Desvende mitos e verdades sobre a necessidade de uma faculdade.',

        bonusTitle2: 'Manual Trabalho Instantâneo',
        bonusDesc2: 'Descubra onde encontrar oportunidades e como se destacar no mercado.',
        bonusLil1Desc2: 'Aprenda como transformar seu talento em uma carreira lucrativa.',
        bonusLil2Desc2: 'Descubra quem contrata e onde encontrar trabalho como desenhista.',
        bonusLil3Desc2: 'Avalie se você está pronto para entrar no mercado e como se preparar melhor.',

        bonusTitle3: 'Guia Materiais de Desenho',
        bonusDesc3: 'Saiba onde comprar, comparar preços e escolher os melhores materiais para seu estilo',
        bonusLil1Desc3: 'Conheça as melhores lojas para comprar materiais de desenho no país.',
        bonusLil2Desc3: 'Entenda as diferenças entre material escolar e artístico antes de investir.',
        bonusLil3Desc3: 'Descubra os preços e faça escolhas inteligentes para seu orçamento.',

    },
    {
        id: 2,
        productName: 'Como Desenhar Mangá',
        title: 'ué',
        thumb: "https://kronus.kebook.com.br/assets/5ceb4048-d058-4be9-9622-202c8069e405/content-expert.png",
        archive: "1mPr3qzMEiJ4Rmhtjqmw-LPS1rc0D0jby"
    },
    {
        id: 3,
        productName: 'Como Desenhar Quadrinhos',
        title: 'ué',
        thumb: "https://kronus.kebook.com.br/assets/55bc81e1-d7c7-4867-a32c-90913c64962d/content-expert.png",
        archive: "1Nr_LgtSa-P2M9d2rh6iUpsRukA37WscY"
    },
    {
        id: 4,
        title: 'ué',
        productName: 'Pintando com Marcadores',
        thumb: "https://kronus.kebook.com.br/assets/55c25079-1155-4fbc-8cb9-7d950a7f5b7d/content-expert.png",
        archive: "1-X1EVRW8sjNk9hFohLDNoyNBmSGTilOR"
    },
    {
        id: 5,
        title: 'ué',
        productName: 'Desenho Gestual',
        thumb: "https://kronus.kebook.com.br/assets/cdcb5c8d-24ba-4783-bb99-99fa0264b07d/content-expert.png",
        archive: "12zbiXZOxzVLXSMsuqy1_tJK1UJSivsWJ"
    }
]

</script>
<template>
    <section class="flex flex-col items-center justify-center mt-10">
        <AtomTitle :title="'Copys do Spyked'" />
        <div class="w-64 h-64">
            <Carousel>
                <CarouselContent>
                    <CarouselItem v-for="delivery in entregasSpy" :key="delivery.id" class="flex flex-col">
                        <img class="object-cover h-56" :src="delivery.thumb" alt="">
                        <a :href="`https://drive.google.com/uc?export=download&id=${delivery.archive}`">
                            <button
                                class="bg-yellow-500 w-full font-black rounded-b-lg p-2 hover:bg-yellow-600 hover:delay-200">Clica em mim!</button>
                        </a>
                    </CarouselItem>
                </CarouselContent>
                <CarouselPrevious />
                <CarouselNext />
            </Carousel>
        </div>
    </section>
</template>
<style scoped>
.subtitle {
    font-size: 22px;
}
</style>