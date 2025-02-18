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
    { //como desenhar ta ok
        id: 1,
        productName: 'Como Desenhar',
        thumb: "https://kronus.kebook.com.br/assets/8926ea06-fcf6-47c0-9c3a-440c1a3478a6/content-expert.png",
        archive: "1dpm-5fsVt0hRNwtjlBVHGJFkndZ_Jv3a",
        linkTo: "https://testingcomodesenhar.kebook.com.br",

        title: 'Desbloqueie o Artista: Técnicas e Práticas para Excelência em Desenho',

        subtitle: 'Transforme suas ideias em arte, aprenda técnicas de desenho e pratique com experts. Torne-se um desenhista habilidoso e criativo.',

        aboutTitle: 'Aprenda a desenhar! Técnicas básicas até avançadas, com muita prática. Transforme seu traço e expresse arte',
        aboutProduct: 'Você já imaginou capturar o mundo com a ponta do seu lápis? Com o curso Como Desenhar, transformamos sua visão artística em realidade, levando você em uma jornada criativa incrível. Este curso é sua chave de ouro para descobrir os segredos do desenho, desde conceitos fundamentais até técnicas avançadas, acessíveis a todos os níveis de habilidade. Liberte o artista dentro de você!\n\nDesenvolvido pelo Thiago Spyked, nosso curso é um tesouro que oferece conteúdo prático e teórico, meticulosamente planejado para impulsionar sua habilidade e confiança. Exploramos perspectiva, sombreamento, composição e muito mais, tudo em um formato fácil de seguir. Veja seu progresso através de exercícios práticos que transformarão sua capacidade de desenhar em poucas semanas!\n\nNão deixe escapar a oportunidade de brilhar no mundo do desenho. A inscrição no Como Desenhar é uma decisão inteligente para quem deseja elevar sua arte. Espaços são limitados, então garanta seu lugar agora e comece a criar obras que capturam a essência da beleza ao seu redor. Vamos juntos desbloquear seu potencial ilimitado!',

        howTitle1: 'Técnicas Essenciais',
        howDesc1: 'Explore os fundamentos do desenho e aprimore sua técnica com práticas efetivas em nosso curso completo.',

        howTitle2: 'Traços Precisos',
        howDesc2: 'Aprenda técnicas essenciais de desenho com videoaulas detalhadas, guias práticos e feedback constante.',

        howTitle3: 'Traços Expressivos',
        howDesc3: 'Aprimore suas habilidades artísticas aplicando técnicas essenciais e práticas direcionadas, aprendidas em nosso programa, para elevar seus desenhos a um novo patamar de excelência!',

        howTitle4: 'Desenho Prático',
        howDesc4: 'Descubra o universo do desenho e aplique conceitos fundamentais e pratique intensamente.',

        bonusTitle1: 'Guia Essencial para Desmistificar Mitos',
        bonusDesc1: 'Descubra o que o mercado exige e quais caminhos seguir para se tornar um profissional.',
        bonusLil1Desc1: 'Compreenda as diferenças entre cursos e escolha o melhor para você',
        bonusLil2Desc1: 'Descubra o que realmente importa para o mercado de trabalho',
        bonusLil3Desc1: 'Desvende mitos e verdades sobre a necessidade de uma faculdade',

        bonusTitle2: 'Manual do Trabalho Instantâneo',
        bonusDesc2: 'Descubra onde encontrar oportunidades e como se destacar no mercado.',
        bonusLil1Desc2: 'Aprenda como transformar seu talento em uma carreira lucrativa',
        bonusLil2Desc2: 'Descubra quem contrata e onde encontrar trabalho como desenhista',
        bonusLil3Desc2: 'Avalie se você está pronto para entrar no mercado e como se preparar melhor',

        bonusTitle3: 'Lista Exclusiva de Materiais de Desenho',
        bonusDesc3: 'Saiba onde comprar, comparar preços e escolher os melhores materiais para seu estilo.',
        bonusLil1Desc3: 'Conheça as melhores lojas para comprar materiais de desenho no país',
        bonusLil2Desc3: 'Entenda as diferenças entre material escolar e artístico antes de investir',
        bonusLil3Desc3: 'Descubra os preços e faça escolhas inteligentes para seu orçamento',

    },
    { // como desenhar manga
        id: 2,
        productName: 'Como Desenhar Mangá',
        thumb: "https://kronus.kebook.com.br/assets/5ceb4048-d058-4be9-9622-202c8069e405/content-expert.png",
        archive: "1mPr3qzMEiJ4Rmhtjqmw-LPS1rc0D0jby",

        title: 'Desenhe Mangás Como um Mestre: Técnicas Profissionais Reveladas',

        subtitle: 'Descubra os segredos de design dos mangás e eleve suas habilidades artísticas para criar cenas e personagens impactantes',

        aboutTitle: 'Transforme seu Traço e Aprenda a Criar Mangás como um Mestre',
        aboutProduct: 'Descubra os segredos milenares dos mestres japoneses para criar mangás impactantes! Com nosso curso, você aprenderá, passo a passo, como ilustrar mangás com a precisão de um verdadeiro profissional. Desde estruturas corporais dinâmicas até expressões faciais marcantes, nossos módulos são desenhados para desbloquear todo o seu potencial criativo. Não importa se você é um iniciante ou já possui alguma prática, este curso é o mapa para o seu sucesso.\n\nImagine capturar toda a emoção e ação de suas cenas favoritas com suas próprias mãos. Em nosso curso, você explorará técnicas avançadas de movimento e posicionamento que trarão seus personagens para a vida de maneira nunca antes vista! Aprenda como balancear detalhes e energia em cada traço, criando obras que mantêm seus espectadores na borda de seus assentos. Transforme suas ideias em arte que respira, luta e ama com a intensidade do universo do mangá.\n\nAlém disso, mergulhe na arte da pintura e colorização, finalizando suas obras com um toque profissional. Com acesso a tutoriais detalhados e feedback constante, você elevará suas habilidades a um nível onde apenas os grandes artistas chegaram. A oportunidade de transformar sua paixão em uma carreira está a apenas um clique de distância. Inscreva-se agora e comece a criar não apenas desenhos, mas histórias que perdurarão por gerações.',

        howTitle1: 'Estrutura do desenho',
        howDesc1: 'Descubra como ilustrar corpos masculinos e femininos, incluindo a cabeça, detalhes faciais, cabelos, mãos, pés, vestimentas e muito mais',

        howTitle2: 'Posturas e Dinamismo',
        howDesc2: 'Aprenda a representar ângulos e movimentos em seus desenhos, trazendo expressividade e realismo para suas histórias',

        howTitle3: 'Composição de Cenas',
        howDesc3: 'Aprenda a desenvolver cenas de luta, expressões, perspectiva, pontos de fuga e a criar cenários ideais para ilustrar suas histórias',

        howTitle4: 'Colorização',
        howDesc4: 'Explore as melhores técnicas de pintura com lápis de cor e digital, aprendendo a finalizar seus desenhos com realismo e profissionalismo',

        bonusTitle1: 'Speed Paint Lápis de Cor Emiya Shirou',
        bonusDesc1: 'Veja todo o processo, do traço à coloração, e aprimore suas técnicas',
        bonusLil1Desc1: 'Acompanhe um passo a passo detalhado para dominar o lápis de cor',
        bonusLil2Desc1: 'Aprenda técnicas práticas para melhorar seus desenhos rapidamente.',
        bonusLil3Desc1: 'Descubra como alcançar um traço e coloração com nível profissional.',

        bonusTitle2: 'Speed Paint Lápis de Cor Mikasa',
        bonusDesc2: 'Veja o processo completo e aprimore suas técnicas com um personagem exclusivo',
        bonusLil1Desc2: 'Siga um passo a passo detalhado para criar sua própria arte.',
        bonusLil2Desc2: 'Aprenda técnicas práticas para dar vida ao seu desenho',
        bonusLil3Desc2: 'Domine traço e coloração para alcançar um resultado profissional.',

        bonusTitle3: 'História do Mangá',
        bonusDesc3: 'Descubra tudo sobre a evolução do mangá e suas influências no mundo!',
        bonusLil1Desc3: 'Descubra curiosidades fascinantes sobre os bastidores da indústria.',
        bonusLil2Desc3: 'Entenda as práticas e técnicas que moldaram esse estilo artístico',
        bonusLil3Desc3: 'Explore a origem do mangá e como ele se tornou um fenômeno global.',
    },
    { // como desenhar quadrinhos ta ok
        id: 3,
        productName: 'Como Desenhar Quadrinhos',
        thumb: "https://kronus.kebook.com.br/assets/55bc81e1-d7c7-4867-a32c-90913c64962d/content-expert.png",
        archive: "1Nr_LgtSa-P2M9d2rh6iUpsRukA37WscY",

        title: 'Domine a Arte dos Quadrinhos: Crie e Publique Suas Histórias em Passos Simples',

        subtitle: 'Transforme ideias em quadrinhos épicos! Aprenda a criar, ilustrar e publicar suas histórias com nosso curso passo a passo. Torne-se um artista reconhecido',

        aboutTitle: 'Aprenda a criar quadrinhos: do esboço ao sucesso em poucos passos',
        aboutProduct: 'Você é fascinado por mundos onde super-heróis, criaturas fantásticas e histórias emocionantes saltam das páginas? Imagine se essas ideias incríveis viessem da sua mente, ganhassem vida através de seus desenhos! Com nosso curso exclusivo, Como Desenhar Quadrinhos, isso não só é possível como garantido. Através de técnicas simples e eficazes, ensinamos você a criar e ilustrar suas próprias narrativas gráficas, passo a passo. Transforme seus rascunhos em obras de arte publicáveis.\n\nNão é só um curso, é uma jornada de descoberta. Aprenda a estruturar enredos cativantes, personagens memoráveis e cenários impressionantes. Desde conceitos básicos até técnicas avançadas de desenho e coloração digital, cobrimos tudo o que você precisa para se tornar um mestre na arte dos quadrinhos. Mais do que isso, você aprenderá estratégias para divulgar e monetizar seu trabalho, atingindo milhares de fãs ávidos por suas criações. \n\nNão deixe seu talento adormecido! O mercado de quadrinhos está em expansão, e este é o momento perfeito para você brilhar. Com acesso vitalício, suporte contínuo e uma comunidade de aspirantes a artistas como você, não há limites para onde suas histórias podem chegar. Inscreva-se hoje e comece a dar vida às histórias que só você pode contar. Seu futuro como criador de quadrinhos começa agora.',

        howTitle1: 'Quadrinhos Criativos',
        howDesc1: 'Aprenda a criar seus quadrinhos com o passo a passo para desenhar produzir e promover suas histórias incríveis e transforme ideias em arte.',

        howTitle2: 'Criação de Quadrinhos',
        howDesc2: 'Saiba como criar quadrinhos do zero, técnicas de desenho, narrativa visual, produção e estratégias de divulgação no mercado.',

        howTitle3: 'Quadrinhos Avançados',
        howDesc3: 'Descubra como transformar sua paixão por desenhos em realidade e aprenda a criar, produzir e divulgar suas histórias únicas.',

        howTitle4: 'Quadrinhos Vívidos',
        howDesc4: 'Desperte seu talento e traga suas histórias à vida com método de aprendizado que vai do esboço à publicação.',

        // nao tem ponto no titulo
        bonusTitle1: 'Evite erros que prejudicam seus desenhos',
        bonusDesc1: 'Descubra os deslizes mais comuns e aprenda a se destacar.',
        bonusLil1Desc1: 'Aprenda a identificar e corrigir os erros mais comuns.',
        bonusLil2Desc1: 'Descubra como ser bem visto e conquistar mais oportunidades.',
        bonusLil3Desc1: 'Melhore sua abordagem e evite armadilhas que atrapalham seu crescimento',

        bonusTitle2: 'Acesse conteúdos exclusivos e atualizados',
        bonusDesc2: 'Aprenda com lives ao vivo e tenha acesso a explicações completas.',
        bonusLil1Desc2: 'Assista a conteúdos atuais',
        bonusLil2Desc2: 'Acompanhe lives exclusivas com conteúdos sempre atualizados',
        bonusLil3Desc2: 'Ganhe mais de 10h de material extra para acelerar seu aprendizado',

        bonusTitle3: '',
        bonusDesc3: '',
        bonusLil1Desc3: '',
        bonusLil2Desc3: '',
        bonusLil3Desc3: '',
    },
    { // pintando com marcadeores
        id: 4,
        productName: 'Pintando com Marcadores',
        thumb: "https://kronus.kebook.com.br/assets/55c25079-1155-4fbc-8cb9-7d950a7f5b7d/content-expert.png",
        archive: "1-X1EVRW8sjNk9hFohLDNoyNBmSGTilOR",

        title: 'Domine a Arte da Pintura com Marcadores e Transforme Ilustrações em Animes',

        subtitle: 'Transforme suas ilustrações em animes espetaculares com técnicas exclusivas de pintura com marcadores. Descubra o artista em você!',

        aboutTitle: 'Eleve suas ilustrações a arte com técnicas de pintura em Anime!',
        aboutProduct: 'Descubra o caminho mágico para transformar suas ilustrações em obras de arte deslumbrantes com nosso exclusivo Curso de Pintura com Marcadores para Animes! Se você sempre sonhou em dar vida aos seus personagens favoritos com cores vibrantes e técnicas profissionais, seu momento chegou. Neste curso, você aprenderá não apenas a pintar, mas a expressar a essência emocional de cada cena, fazendo suas criações pularem do papel!\n\nInvestir em sua paixão por animes e arte nunca foi tão empolgante! Com técnicas detalhadas e dicas especiais de artistas renomados no mundo do anime, este curso é perfeitamente projetado para iniciantes e avançados. Cada aula é uma porta para um universo onde você é o criador de incríveis histórias visuais. Imagine as incríveis texturas que você poderá criar e os efeitos impressionantes que aprenderá a fazer com simples marcadores!\n\nNão espere mais para transformar sua habilidade artística e impressionar todos ao seu redor. As vagas são limitadas, então agarre esta oportunidade única e inscreva-se agora! Prepare-se para ser o artista que sempre quis ser, criando animes que capturam corações e mentes. Este curso é o seu segredo para se destacar e ser reconhecido no emocionante mundo da arte anime. Venha pintar seu caminho para o sucesso!',

        howTitle1: 'Noções Básicas',
        howDesc1: 'Aprenda a escolher e comprar seus marcadores, descubra as melhores combinações de cores, conheça os tipos de papéis ideais e pratique com exercícios para dominar as técnicas ensinadas',

        howTitle2: 'Colorização de Pele',
        howDesc2: 'Entenda o funcionamento e a organização dos marcadores, suas nomenclaturas específicas e aprenda a criar a pele de dois personagens icônicos utilizando as técnicas ensinadas',

        howTitle3: 'Detalhes dos Olhos',
        howDesc3: 'Aprenda a colorir olhos de forma vibrante e expressiva, adicionando profundidade e realismo aos seus personagens.',

        howTitle4: 'Colorização de Roupas',
        howDesc4: 'Aprenda a pintar vestimentas com dobras realistas, descubra as melhores técnicas e saiba como alcançar um acabamento impecável na roupa dos seus personagens.',

        bonusTitle1: 'Line Art na ilustração',
        bonusDesc1: 'Aprenda como funciona a técnica e confira uma inspiração fantástica para você criar suas próprias obras',
        bonusLil1Desc1: 'Domine a partir de uma imagem referência, os conceitos para fazer a Line Art do personagem',
        bonusLil2Desc1: 'Saiba a importância de entender o sentido da luz e o distanciamento para desenvolver uma arte final em seus desenhos',
        bonusLil3Desc1: 'Consiga aplicar em suas próprias criações os ensinamentos demonstrados neste conteúdo',

        bonusTitle2: 'Pintura de cabelo em tempo real',
        bonusDesc2: 'Acompanhe a segunda parte e a finalização da pintura iniciada na aula três do curso',
        bonusLil1Desc2: 'Confira na íntegra como o expert resolve essa pintura exclusiva em tempo real',
        bonusLil2Desc2: 'Acesse um conteúdo sem aceleração e com áudio mutado para você ficar mais confortável escutando o que quiser',
        bonusLil3Desc2: 'Domine a pintura com marcadores para o cabelo da personagem com todas as técnicas, nuances e métodos utilizados',

        bonusTitle3: 'Pintura de luva em tempo real',
        bonusDesc3: 'Aprenda como pintar a luva do personagem Saitama de One Punch-Man do início ao fim',
        bonusLil1Desc3: 'Confira mais um conteúdo inédito, completo e exclusivo para te ajudar em seus estudos práticos',
        bonusLil2Desc3: 'Acompanhe este processo de pintura com todo o conforto necessário para seu melhor aprendizado',
        bonusLil3Desc3: 'Encontre um novo desafio de pintura e coloque em prática com todas as dicas, ensinamentos e orientações do curso',
    },
    {
        id: 5,
        productName: 'Desenho Gestual',
        thumb: "https://kronus.kebook.com.br/assets/cdcb5c8d-24ba-4783-bb99-99fa0264b07d/content-expert.png",
        archive: "12zbiXZOxzVLXSMsuqy1_tJK1UJSivsWJ",

        title: 'Desbloqueie a Arte do Movimento: Curso Prático de Desenho Gestual',

        subtitle: 'Transforme seus traços! Participe do curso de desenho gestual e aprenda, na prática, a dar vida e movimento aos seus desenhos artísticos',

        aboutTitle: 'Aprenda Técnicas de Desenho Gestual e Dê Vida aos Seus Traços!',
        aboutProduct: 'Você está pronto para transformar seus desenhos e dar vida às suas criações de uma maneira que jamais imaginou? O nosso Curso de Desenho Gestual é a chave para desbloquear o potencial oculto em cada traço, proporcionando dinamismo e fluidez que vão fazer suas obras saltarem do papel. Este curso exclusivo está alinhado com as mais recentes técnicas de movimento, garantindo que você aprenda através da prática direcionada e eficaz.\n\nImagine capturar a essência do movimento humano em cada linha, criando obras que não apenas representam, mas que também respiram e se movem com uma naturalidade impressionante! Conosco, você vai absorver cada segredo para aplicar esse conhecimento em qualquer estilo de desenho que desejar. Nossos módulos são projetados para lhe proporcionar uma experiência de aprendizado intensa e gratificante, que eleva sua habilidade ao próximo nível.\n\nNão deixe essa oportunidade única escapar! Junte-se a uma comunidade de artistas talentosos que, como você, desejam se aprofundar no universo do desenho gestual e revolucionar sua forma de expressão artística. Inscreva-se agora e seja parte desse movimento artístico, onde cada gesto transforma papel e tinta em puro encanto!',

        howTitle1: 'Tridimensionalidade',
        howDesc1: 'Descubra como trazer mais realismo e dinamismo aos seus desenhos com técnicas em 3D e eleve seu nível como artista',

        howTitle2: 'Composição da Figura Humana',
        howDesc2: 'Aprenda a criar a figura humana de forma fluida e natural, eliminando a rigidez e ganhando liberdade e expressividade nos seus desenhos.',

        howTitle3: 'Gestos Dinâmicos',
        howDesc3: 'Aprimore sua arte com nosso curso de desenho gestual! Aprenda técnicas práticas para infundir movimento e vida em cada traço e transforme suas criações visuais.',

        howTitle4: 'Método Simplificado',
        howDesc4: 'Acesse um conteúdo claro, completo, exclusivo e eficiente para acompanhar e facilitar sua jornada no aprendizado',

        bonusTitle1: '',
        bonusDesc1: '',
        bonusLil1Desc1: '',
        bonusLil2Desc1: '',
        bonusLil3Desc1: '',

        bonusTitle2: '',
        bonusDesc2: '',
        bonusLil1Desc2: '',
        bonusLil2Desc2: '',
        bonusLil3Desc2: '',

        bonusTitle3: '',
        bonusDesc3: '',
        bonusLil1Desc3: '',
        bonusLil2Desc3: '',
        bonusLil3Desc3: '',
    }
]

const showModal = ref(false);
const selectedDelivery = ref<any>(null);

const openModal = (delivery: any) => {
  selectedDelivery.value = delivery;
  showModal.value = true;
};

const closeModal = () => {
  showModal.value = false;
};
</script>
<template>
    <section class="flex flex-col items-center justify-center mt-10">
        <AtomTitle :title="'Copys do Spyked'" />
        <div class="w-64 h-64">
            <Carousel>
                <CarouselContent>
                    <CarouselItem v-for="delivery in entregasSpy" :key="delivery.id" class="flex flex-col">
                        <img 
                            class="object-cover h-56 cursor-pointer" 
                            :src="delivery.thumb" 
                            alt=""
                            @click="openModal(delivery)"
                        >
                        <a :href="`https://drive.google.com/uc?export=download&id=${delivery.archive}`">
                            <button
                                class="bg-yellow-500 w-full font-black rounded-b-lg p-2 hover:bg-yellow-600 hover:delay-200">
                                Clica em mim!
                            </button>
                        </a>
                    </CarouselItem>
                </CarouselContent>
                <CarouselPrevious />
                <CarouselNext />
            </Carousel>
        </div>

        <!-- Modal -->
        <div v-if="showModal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 z-50"
            @click.self="closeModal">
            <div class="bg-white rounded-lg max-w-2xl max-h-[90vh] w-full overflow-hidden flex flex-col">
                <div class="flex justify-between items-center p-4 border-b">
                    <h2 class="text-xl font-bold">{{ selectedDelivery.productName }}</h2>
                    <button @click="closeModal" class="text-gray-500 hover:text-gray-700">
                        ✕
                    </button>
                </div>
                
                <div class="overflow-y-auto p-4 space-y-6">
                    <!-- Seção Principal -->
                    <div v-if="selectedDelivery.title">
                        <span>Título principal:</span>
                        <h3 class="text-lg font-semibold mb-2">{{ selectedDelivery.title }}</h3>
                        <span>Subtítulo:</span>
                        <p class="text-gray-600">{{ selectedDelivery.subtitle }}</p>
                    </div>

                    <!-- Sobre o Produto -->
                    <div v-if="selectedDelivery.aboutTitle">
                        <span>Título em cima da descrição sobre o curso:</span>
                        <h3 class="font-bold mb-2">{{ selectedDelivery.aboutTitle }}</h3>
                        <span>Descrição completa do curso:</span>
                        <p class="text-gray-600 whitespace-pre-line">{{ selectedDelivery.aboutProduct }}</p>
                    </div>


                    <!-- Métodos -->
                    <div v-for="(_, index) in 4" :key="index" class="mt-0">
                        <span>{{`How ${index + 1}:`}}</span>
                        <div v-if="selectedDelivery[`howTitle${index + 1}`]">
                            <h4 class="font-semibold mt-4">{{ selectedDelivery[`howTitle${index + 1}`] }}</h4>
                            <p class="text-gray-600">{{ selectedDelivery[`howDesc${index + 1}`] }}</p>
                        </div>
                    </div>

                    <!-- Bônus -->
                    <div v-for="(_, index) in 3" :key="`bonus-${index}`">
                        <span>{{`Bônus ${index + 1}:`}}</span>
                        <div v-if="selectedDelivery[`bonusTitle${index + 1}`]">
                            <h3 class="font-bold mt-6 text-lg">{{ selectedDelivery[`bonusTitle${index + 1}`] }}</h3>
                            <p class="text-gray-600 mb-2">{{ selectedDelivery[`bonusDesc${index + 1}`] }}</p>
                            <ul class="list-disc pl-6 space-y-2">
                                <li v-if="selectedDelivery[`bonusLil1Desc${index + 1}`]">
                                    {{ selectedDelivery[`bonusLil1Desc${index + 1}`] }}
                                </li>
                                <li v-if="selectedDelivery[`bonusLil2Desc${index + 1}`]">
                                    {{ selectedDelivery[`bonusLil2Desc${index + 1}`] }}
                                </li>
                                <li v-if="selectedDelivery[`bonusLil3Desc${index + 1}`]">
                                    {{ selectedDelivery[`bonusLil3Desc${index + 1}`] }}
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>

                <div class="p-4 border-t flex justify-end space-x-7">
                    <a v-if="selectedDelivery.linkTo" :href="selectedDelivery.linkTo" class="px-4 py-2 bg-yellow-200 hover:bg-yellow-300 rounded-lg">Ver Online</a>
                    <button 
                        @click="closeModal"
                        class="px-4 py-2 bg-gray-200 hover:bg-gray-300 rounded-lg"
                    >
                        Fechar
                    </button>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
.subtitle {
    font-size: 22px;
}

.modal-content {
    max-height: 80vh;
}
span {
    color: red;
}
</style>