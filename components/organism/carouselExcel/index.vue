<script setup lang="ts">
import AtomTitle from '~/components/atoms/atomTitle/atomTitle.vue';
import {
    Carousel,
    CarouselContent,
    CarouselItem,
    CarouselNext,
    CarouselPrevious,
} from '@/components/ui/carousel'

const entregasExcel = [
    {//Curso de Excel Online
        id: 1,
        productName: 'Curso de Excel Online',
        thumb: "https://kronus.kebook.com.br/assets/3cd3d543-0b65-4cff-a2c4-8ec2dc41678c/content-expert.png",
        archive: "",

        title: 'Aprenda a criar planilhas, controlar estoque e finanças, calcular comissões e mais. Torne-se um expert em análise de dados',

        subtitle: 'Transforme números em sucesso e descubra como Excel pode elevar seu potencial analítico e gerencial desde iniciante até avançado',

        aboutTitle: 'Desbloqueie o Potencial do Excel: Técnicas Avançadas e Práticas',
        aboutProduct: 'Descubra o caminho para a eficiência e destaque no mercado com o nosso Curso de Excel Online! Se o segredo da produtividade é dominar as ferramentas certas, estar preparado para todas as demandas do Office irá elevar sua performance profissional a patamares inimagináveis! Neste curso, você irá aprender tudo sobre planilhas, gestão de estoques, controle financeiro e muito mais.\n\nImagine ser capaz de agilizar todos os seus processos, criando relatórios detalhados, gráficos impactantes e calculando taxas e comissões com precisão cirúrgica. Com nosso treinamento, essa realidade está ao seu alcance! Não perca a oportunidade de adquirir habilidades críticas que elevarão seu valor no mercado de trabalho, tornado-o indispensável em qualquer equipe.\n\nNão deixe para depois a chance de transformar sua carreira com conhecimentos que colocarão você à frente de muitos profissionais. Inscreva-se agora e garanta acesso imediato aos conteúdos e técnicas que têm o poder de abrir novos horizontes em sua vida profissional. É a sua vez de brilhar com excelência no uso do Excel!\n',

        howTitle1: 'Gestão de Qualidade',
        howDesc1: 'Domine diferentes tipos de planilhas profissionais, amplamente utilizadas por administradores, gestores e executivos, para otimizar a gestão e o controle de qualidade.',

        howTitle2: 'Do Básico ao Avançado',
        howDesc2: 'Explore as diversas ferramentas e funções do Excel, saindo rapidamente do nível iniciante para o avançado de forma simples e eficiente.',

        howTitle3: 'Habilidades Profissionais',
        howDesc3: 'Aprenda a inserir, localizar, filtrar, editar e proteger dados em planilhas, gráficos, tabelas e muito mais, para aprimorar suas habilidades profissionais',

        howTitle4: 'Potencial do Excel',
        howDesc4: 'Descubra o poder do Excel com nosso curso online! Aprenda a criar planilhas detalhadas, controlar estoques e gastos, gerenciar clientes, calcular comissões e muito mais',

        bonusTitle1: 'Masterclass: Torne-se um Consultor Expert em Excel',
        bonusDesc1: 'Descubra os passos essenciais para ganhar dinheiro oferecendo serviços profissionais em Excel.',
        bonusLil1Desc1: 'Entenda o mercado e a alta demanda por serviços de Excel',
        bonusLil2Desc1: 'Domine os conhecimentos necessários para atuar na área',
        bonusLil3Desc1: 'Aprenda a analisar e se destacar da concorrência',

        bonusTitle2: 'Domine Tudo Sobre Gráficos Dinâmicos no Excel',
        bonusDesc2: 'Um estudo completo e detalhado sobre gráficos dinâmicos, com exemplos práticos para você se destacar.',
        bonusLil1Desc2: 'Utilize controles de formulários e ActiveX em gráficos',
        bonusLil2Desc2: 'Explore diversos tipos de gráficos e suas aplicações',
        bonusLil3Desc2: 'Aprenda a criar Dashboards profissionais e impactantes',

        bonusTitle3: 'Infográficos Impactantes para Apresentações no PowerPoint',
        bonusDesc3: 'Aprenda a usar as ferramentas do PowerPoint para criar apresentações impecáveis e cheias de impacto.',
        bonusLil1Desc3: 'Mais de 4 horas e meia de conteúdo prático e detalhado',
        bonusLil2Desc3: 'Domine os conceitos-chave para criar infográficos de alto nível',
        bonusLil3Desc3: 'Descubra como fazer apresentações profissionais com diversas ferramentas poderosas',
    },
    {//Quero Aprender Dashboard
        id: 2,
        productName: 'Aula: Como Criar um Dashboard',
        thumb: "https://kronus.kebook.com.br/assets/c6aa3ce7-c296-43a4-bc75-1b21b95d4b5a/content-expert.png",
        archive: "",

        title: 'Aula para Criar Dashboards Dinâmicos no Excel Transforme Dados em Decisões ',

        subtitle: 'Transforme seu Excel e aprenda a criar dashboards dinâmicos e torne a análise de dados rápida e eficaz. Eleve suas habilidades e impulsione sua carreira',

        aboutTitle: 'Transforme Dados em Decisões com Dashboards no Excel',
        aboutProduct: 'Descubra o poder do Excel e transforme suas planilhas em dashboards dinâmicos que simplificam decisões! Em nossa aula exclusiva, você será guiado passo a passo na arte de construir dashboards visuais e interativos. Esqueça aquelas horas perdidas tentando interpretar números complexos e aprenda a criar ferramentas que destacam o essencial, agilizando sua análise de dados.\n\nEsteja você buscando impressionar na sua próxima apresentação de negócios ou apenas quer otimizar a gestão de seus projetos pessoais, nosso aula é a chave para desbloquear todo o potencial do Excel. Com técnicas práticas e eficazes, ensinamos você a transformar dados brutos em informações claras e precisas, faciltando a interpretação e a tomada de decisões.\n\nNão perca a chance de elevar seu nível profissional com habilidades de alto valor no mercado. Inscreva-se agora e comece a construir dashboards que não apenas organizam, mas também revelam caminhos e soluções, todas as vezes que você abrir sua planilha. Vagas limitadas para um aprendizado que colocará você à frente no mundo dos dados!',

        howTitle1: 'Dashboards Eficientes',
        howDesc1: 'Aprenda a criar dashboards no Excel para uma análise de dados rápida, clara e eficiente, e transforme suas planilhas',

        howTitle2: 'Dashboards Dinâmicos',
        howDesc2: 'Descubra técnicas de Excel para criar dashboards eficazes, utilizando gráficos interativos e funções avançadas, tornando suas análises de dados claras e práticas',

        howTitle3: 'Excel Avançado',
        howDesc3: 'Aprenda a transformar conhecimentos do aula em dashboards dinâmicos no Excel, facilitando a análise e visibilidade dos seus dados, e torne suas planilhas incrivelmente eficientes',

        howTitle4: 'Excel Dinâmico',
        howDesc4: 'Descubra as técnicas para transformar suas planilhas: aprenda a criar dashboards no Excel e visualize seus dados de forma clara e eficiente',

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
    },
    {//Aula: Tudo sobre Função SE
        id: 3,
        productName: 'Aula: Tudo sobre Função SE',
        thumb: "https://kronus.kebook.com.br/assets/a6f95149-ab00-49be-9d75-5690a4581d20/content-expert.png",
        archive: "",

        title: 'Domine a Função SE: Acelere sua Produtividade em Excel Sem Estresse',

        subtitle: 'Domine a função SE no Excel, otimize análises e impulsione sua eficiência! Torne-se um expert e economize horas com nossas técnicas exclusivas.',

        aboutTitle: 'Domine a Função SE: Acelere Sua Produtividade em Excel',
        aboutProduct: 'Descubra o segredo para dominar análises complexas e incrementar sua produtividade com a nossa aula revolucionário: “Tudo sobre Função SE”! Esta aula é a chave mágica que abrirá as portas para você entender de maneira simples e eficaz como utilizar a Função SE em Excel, tornando-se um mestre na criação de comparações lógicas. Não perca mais tempo com dúvidas e indecisões — se você busca eficiência, este é o caminho!\n\nImagine poder, em poucas horas, adquirir habilidades que muitos levam anos para desenvolver. Com técnicas passo a passo, nossa aula é desenhado para fornecer uma aprendizagem acelerada que se adapta ao seu ritmo. Ao dominar a Função SE, você não apenas aumenta sua capacidade de resolver problemas complexos, mas também se destaca no mercado de trabalho. Esta é a sua chance de brilhar e mostrar seu verdadeiro potencial!\n\nNão fique para trás na corrida pela excelência profissional. Garanta já sua vaga nesse curso transformador e comece a transformar seu futuro hoje mesmo! Com exemplos práticos, você vai aprender a aplicar a Função SE de forma surpreendentemente simples e eficiente, garantindo mais tempo e melhores resultados em seus projetos. A oportunidade está batendo à sua porta, abra-a para um mundo de possibilidades e sucesso. Inscreva-se agora e dê o primeiro passo para se tornar um verdadeiro especialista em Excel!',

        howTitle1: 'Exercícios Práticos',
        howDesc1: 'Aprenda fazendo! Resolva exercícios para consolidar os conceitos da aula e ganhe confiança na aplicação do seu conhecimento.',

        howTitle2: 'Capacitação Profissional',
        howDesc2: 'Aprenda com especialistas, adquira as habilidades necessárias para o mercado de trabalho e alcance o emprego dos seus sonhos.',

        howTitle3: 'Aperfeiçoamento em Excel',
        howDesc3: 'Entenda tudo sobre a função SE, avance seus conhecimentos sobre Excel e aproxime-se de um uso completo e eficiente da ferramenta.',

        howTitle4: 'Domine SE',
        howDesc4: 'Descubra como dominar a função SE no Excel! Simplifique suas comparações lógicas, aumente sua produtividade e economize tempo com nosso infoproduto exclusivo.',

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
    },
    {//Aula: Domine o ProcV
        id: 4,
        productName: 'Aula: Domine o ProcV',
        thumb: "https://kronus.kebook.com.br/assets/b8c4afd0-d80c-4597-ad71-a0d687877734/content-expert.png",
        archive: "",

        title: '',

        subtitle: '',

        aboutTitle: '',
        aboutProduct: '',

        howTitle1: '',
        howDesc1: '',

        howTitle2: '',
        howDesc2: '',

        howTitle3: '',
        howDesc3: '',

        howTitle4: '',
        howDesc4: '',

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
    },
    {//Teste de Excel para Entrevista
        id: 5,
        productName: 'Teste de Excel para Entrevista',
        thumb: "https://kronus.kebook.com.br/assets/2e8e8220-c303-416b-80c6-3b138b7de4d7/content-expert.png",
        archive: "",

        title: '',

        subtitle: '',

        aboutTitle: '',
        aboutProduct: '',

        howTitle1: '',
        howDesc1: '',

        howTitle2: '',
        howDesc2: '',

        howTitle3: '',
        howDesc3: '',

        howTitle4: '',
        howDesc4: '',

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
    },
    {//Aula: Excel para Assistente Adminsitrativo
        id: 6,
        productName: 'Aula: Excel para Assistente Adminsitrativo',
        thumb: "https://kronus.kebook.com.br/assets/a9afd1ee-5796-440c-9be8-84f55052d7c8/content-expert.png",
        archive: "",

        title: '',

        subtitle: '',

        aboutTitle: '',
        aboutProduct: '',

        howTitle1: '',
        howDesc1: '',

        howTitle2: '',
        howDesc2: '',

        howTitle3: '',
        howDesc3: '',

        howTitle4: '',
        howDesc4: '',

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
    },
    {//Curso de Planilhas Google
        id: 7,
        productName: 'Curso de Planilhas Google',
        thumb: "https://kronus.kebook.com.br/assets/644f8f10-a61e-41d7-a32c-ece14498f860/content-expert.png",
        archive: "",

        title: '',

        subtitle: '',

        aboutTitle: '',
        aboutProduct: '',

        howTitle1: '',
        howDesc1: '',

        howTitle2: '',
        howDesc2: '',

        howTitle3: '',
        howDesc3: '',

        howTitle4: '',
        howDesc4: '',

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
    },
    {//Curso primeiros passos no Excel
        id: 8,
        productName: 'Curso primeiros passos no Excel',
        thumb: "https://kronus.kebook.com.br/assets/0c7d2bb2-aac5-451c-88e1-2ee5d059485f/content-expert.png",
        archive: "",

        title: '',

        subtitle: '',

        aboutTitle: '',
        aboutProduct: '',

        howTitle1: '',
        howDesc1: '',

        howTitle2: '',
        howDesc2: '',

        howTitle3: '',
        howDesc3: '',

        howTitle4: '',
        howDesc4: '',

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
    },
    {//Cursos Planilhas de Excel
        id: 9,
        productName: 'Cursos Planilhas de Excel',
        thumb: "https://kronus.kebook.com.br/assets/8716a1fd-9232-4dcc-bd5d-0c67955c4904/content-expert.png",
        archive: "",

        title: '',

        subtitle: '',

        aboutTitle: '',
        aboutProduct: '',

        howTitle1: '',
        howDesc1: '',

        howTitle2: '',
        howDesc2: '',

        howTitle3: '',
        howDesc3: '',

        howTitle4: '',
        howDesc4: '',

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
                    <CarouselItem v-for="delivery in entregasExcel" :key="delivery.id" class="flex flex-col">
                        <img 
                            class="object-cover h-56 cursor-pointer" 
                            :src="delivery.thumb" 
                            alt=""
                            @click="openModal(delivery)"
                        >
                        <a :href="`https://drive.google.com/uc?export=download&id=${delivery.archive}`">
                            <button
                                class="bg-green-500 w-full font-black rounded-b-lg p-2 hover:bg-green-600 hover:delay-200">
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