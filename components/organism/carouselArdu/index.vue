<script setup lang="ts">
import AtomTitle from '~/components/atoms/atomTitle/atomTitle.vue';
import {
    Carousel,
    CarouselContent,
    CarouselItem,
    CarouselNext,
    CarouselPrevious,
} from '@/components/ui/carousel'

const entregasSpy = [
    { //arduino 2.0
        id: 1,
        productName: 'Arduino 2.0',
        thumb: "https://kronus.kebook.com.br/assets/0a17ebc3-8b5b-436b-aac9-af2ae925ad53/content-expert.png",
        archive: "",
        linkTo: "https://testingcursodearduino.kebook.com.br/",

        title: 'Aprenda Arduino do zero programe com facilidade e desenvolva projetos inovadores que impressionam',

        subtitle: 'Aprenda Arduino rápido e crie soluções high-tech que impressionam, mesmo iniciando agora',

        aboutTitle: 'Descubra como programar Arduino e crie projetos incríveis, mesmo sem experiência prévia',
        aboutProduct: 'Imagine um mundo onde você pode criar dispositivos inteligentes, automatizar tarefas do dia a dia e dar vida a projetos incríveis com suas próprias mãos. Com o Curso de Arduino, esse poder está ao seu alcance! Aqui, você vai aprender a programar de forma simples e prática, mesmo que nunca tenha escrito uma linha de código. De robôs a sistemas de automação residencial, as possibilidades são infinitas – e tudo começa com o primeiro passo que você der hoje.\nEste curso foi desenvolvido para iniciantes e entusiastas que desejam ir além da teoria e colocar a mão na massa. Com aulas didáticas, exemplos reais e projetos passo a passo, você vai adquirir habilidades que impressionam. Imagine a satisfação de ver seu primeiro projeto funcionando perfeitamente, ou até mesmo apresentar uma solução inovadora para amigos, familiares ou no mercado de trabalho. O Arduino é a ferramenta do futuro, e você está a um clique de fazer parte dessa revolução.\nNão importa se você é um estudante, hobbyista ou profissional em busca de novas habilidades – este curso é o atalho para o sucesso. Com acesso vitalício, suporte especializado e uma comunidade de makers como você, não há limites para o que pode alcançar. Não espere mais para transformar suas ideias em realidade. Inscreva-se agora e comece a criar projetos que vão mudar sua vida e a de quem está ao seu redor. O futuro é seu para construir!',

        howTitle1: 'Aprenda a Programar',
        howDesc1: 'Crie projetos incríveis e automatize soluções inteligentes, mesmo sem experiência prévia. Transforme ideias em realidade',

        howTitle2: 'Crie Projetos',
        howDesc2: 'Desenvolva projetos inovadores, desde automação residencial até robótica, mesmo começando do zero. Seu futuro criativo começa aqui',

        howTitle3: 'Arduino Básico',
        howDesc3: 'Aprenda os conceitos fundamentais do Arduino, desde a estrutura do hardware até a lógica de programação, e comece a criar seus primeiros projetos com confiança',

        howTitle4: 'Progresso no Arduino',
        howDesc4: 'Do básico ao avançado: aprenda a programar Arduino, entenda componentes eletrônicos e crie projetos complexos, evoluindo de iniciante a expert em pouco tempo',

        bonusTitle1: 'Qual Modelo de Arduino Comprar: Guia Prático para Iniciantes',
        bonusDesc1: 'Descubra por onde começar e escolha o modelo ideal de Arduino para seus projetos',
        bonusLil1Desc1: 'Orientação prática para iniciantes',
        bonusLil2Desc1: 'Aprenda como escolher o Arduino certo para suas necessidades',
        bonusLil3Desc1: 'Conheça as diferenças entre os modelos e suas aplicações',

        bonusTitle2: 'Transforme Projetos com Arduino em Produtos Profissionais',
        bonusDesc2: 'Aprenda a lucrar e se tornar um profissional, transformando suas ideias em produtos de sucesso',
        bonusLil1Desc2: 'Domine o passo a passo para iniciar e finalizar projetos profissionais',
        bonusLil2Desc2: 'Acesse vídeos completos com todas as explicações detalhadas',
        bonusLil3Desc2: 'Descubra estratégias para monetizar seus projetos com Arduino',

        bonusTitle3: 'Proteja seu Projeto com Arduino Contra Pirataria',
        bonusDesc3: 'Aprenda os conceitos fundamentais de segurança para garantir a integridade dos seus projetos',
        bonusLil1Desc3: 'Desenvolva um Arduino com proteção anti-pirataria',
        bonusLil2Desc3: 'Siga um passo a passo completo e prático',
        bonusLil3Desc3: 'Aprenda técnicas avançadas para blindar seus projetos',

    },
    { //corte a laser
        id: 2,
        productName: 'Guia do Corte a Laser',
        thumb: "https://kronus.kebook.com.br/assets/f14174eb-cef9-41c8-bf3f-2e6664dbe92c/content-expert.png",
        archive: "",
        linkTo: "",

        title: 'Transforme Ideias em Realidade do Tinkercad ao Corte a Laser, Crie Projetos Incríveis com Precisão Profissional',

        subtitle: 'Aprenda a criar do zero: da modelagem 3D no Tinkercad ao corte a laser, produza peças precisas e impressionantes como um verdadeiro maker',

        aboutTitle: 'Do design 3D ao corte a laser: crie peças profissionais e torne-se um expert maker em poucos passos',
        aboutProduct: 'Imagine transformar suas ideias em peças reais, com precisão e qualidade profissional, usando uma das tecnologias mais incríveis do mundo maker: o corte a laser. Com este curso, você vai dominar todas as etapas, desde a modelagem 3D no Tinkercad até a produção final na máquina de corte e gravação a laser. Não importa se você é um iniciante ou já tem alguma experiência – aqui, você vai aprender de forma prática, rápida e eficiente, com um método que vai levar suas habilidades a um novo patamar.\nEste curso foi desenvolvido para quem quer ir além da teoria e colocar a mão na massa. Você vai aprender a criar designs incríveis, configurar a máquina de corte a laser e produzir peças que impressionam. De projetos pessoais a soluções profissionais, as possibilidades são infinitas. Imagine a satisfação de ver suas criações ganhando vida, com detalhes precisos e acabamento impecável. Este é o seu momento de se tornar um verdadeiro maker e transformar sua criatividade em realidade!\nCom acesso vitalício, suporte especializado e uma comunidade de makers para trocar ideias, você terá tudo o que precisa para evoluir rapidamente. Não espere mais para começar a criar peças únicas e funcionais que vão destacar seu trabalho. Inscreva-se agora e dê o primeiro passo para dominar o corte a laser e se tornar um expert na arte da criação digital. O futuro da fabricação está em suas mãos – comece hoje mesmo!',
        
        howTitle1: 'Corte Criativo',
        howDesc1: 'Aprenda a criar peças incríveis, desde a modelagem 3D no Tinkercad até o corte e gravação final na máquina a laser, e transforme suas ideias em realidade',

        howTitle2: 'Finalize Projetos',
        howDesc2: 'Domine todas as etapas, da modelagem 3D no Tinkercad ao corte e gravação a laser, e finalize seus projetos com precisão e qualidade profissional',

        howTitle3: 'Cuidados Essenciais',
        howDesc3: 'Aprenda os cuidados imprescindíveis para trabalhar com corte a laser, desde a modelagem 3D no Tinkercad até a finalização segura e eficiente do seu projeto',

        howTitle4: 'Iniciando no Laser',
        howDesc4: 'Descubra o passo a passo completo para iniciantes, desde a modelagem 3D no Tinkercad até o corte e gravação a laser, e comece a criar seus projetos com confiança',

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
    { //arduino principainte
        id: 3,
        productName: 'Arduino Principiantes',
        thumb: "https://kronus.kebook.com.br/assets/e0784530-0fb5-47cf-8f10-d8e791e6d1fd/content-expert.png",
        archive: "",
        linkTo: "",

        title: 'Descubra o Arduino Aprenda Programação e Crie Projetos Incríveis Mesmo Começando do Zero',

        subtitle: 'Do zero ao criador: aprenda Arduino de forma simples, programe como um expert e desenvolva projetos inovadores que impressionam',

        aboutTitle: 'Descubra como programar Arduino e crie projetos incríveis, mesmo sem experiência prévia. Comece agora e transforme suas ideias em realidade',
        aboutProduct: 'Já imaginou criar projetos incríveis com suas próprias mãos, dando vida a ideias inovadoras? Com o Curso de Arduino para Iniciantes, você aprende do zero a programar e dominar os conceitos essenciais da eletrônica e automação. Mesmo sem experiência, em poucas aulas, você estará desenvolvendo circuitos inteligentes e controlando dispositivos com facilidade!\n100% prático, didático e sem enrolação! Aprenda a programar, conectar sensores, criar sistemas automatizados e muito mais! Com suporte direto de especialistas e materiais exclusivos, você transforma seu aprendizado em algo simples e divertido.\nNão perca essa oportunidade de entrar no mundo da tecnologia! Inscreva-se agora e comece a criar seus próprios projetos inovadores com Arduino. Seja para hobby, profissão ou negócios, esse é o primeiro passo para dominar a eletrônica e a programação! ',

        howTitle1: 'Arduino Básico',
        howDesc1: 'Aprenda os conceitos fundamentais e comece a programar em Arduino de forma simples e prática, criando seus primeiros projetos eletrônicos com confiança',

        howTitle2: 'Prática Eletrônica',
        howDesc2: 'Pratique bastante e domine a programação em Arduino! Aprenda os conceitos básicos e desenvolva projetos eletrônicos de forma hands-on e eficiente',

        howTitle3: 'Autonomia Profissional',
        howDesc3: 'Ganhe autonomia profissional com Arduino! Aprenda a programar e desenvolver projetos eletrônicos completos, desde os conceitos básicos até aplicações avançadas.',

        howTitle4: 'Programação Prática',
        howDesc4: 'Aprenda de forma hands-on a criar projetos eletrônicos funcionais e desenvolva suas habilidades de programação',

        bonusTitle1: 'Guia Completo de Montagem da Garra do Braço Robótico',
        bonusDesc1: 'Aprenda a montar a garra do braço robótico com um guia detalhado e prático',
        bonusLil1Desc1: 'Entenda o funcionamento dos motores e sua aplicação na garra',
        bonusLil2Desc1: 'Lista de materiais necessários e esquema de identificação das peças',
        bonusLil3Desc1: 'Passo a passo para a conexão da garra e do servo motor',

        bonusTitle2: 'Aulão de Solda: Técnicas para Componentes e Fios',
        bonusDesc2: 'Aprenda a realizar soldas seguras e precisas para seus projetos robóticos',
        bonusLil1Desc2: 'Conheça as ferramentas essenciais para soldagem',
        bonusLil2Desc2: 'Dicas de segurança para soldar fios e componentes com confiança',
        bonusLil3Desc2: 'Passo a passo detalhado para criar conexões perfeitas e duráveis',

        bonusTitle3: 'Montagem do Robô 2WD: Do Zero ao Funcionamento',
        bonusDesc3: 'Aprenda a montar seu robô de duas rodas desde o início, com instruções detalhadas e práticas',
        bonusLil1Desc3: 'Passo a passo completo da montagem do kit',
        bonusLil2Desc3: 'Dicas e cuidados essenciais para a instalação dos motores',
        bonusLil3Desc3: 'Como utilizar decoders para regular a tensão de alimentação com precisão',

        bonusTitle4: 'Robô EasyRoverDS: Acionamento e Montagem',
        bonusDesc4: 'Explore sugestões de códigos de acionamento e domine a montagem do robô EasyRoverDS',
        bonusLil1Desc4: 'Manual completo com esquema detalhado de montagem',
        bonusLil2Desc4: 'Planos da plataforma robótica em spumapaper para construção precisa',
        bonusLil3Desc4: 'Tutorial passo a passo para modificar o servo Turnigy Tg9e',

    },
    { //guia de referencia arduino
        id: 4,
        productName: 'Guia de referencia arduino',
        thumb: "https://kronus.kebook.com.br/assets/793fb542-407c-41da-81b2-1ca7f658486b/content-expert.png",
        archive: "",
        linkTo: "",

        title: 'Guia Essencial do Arduino: Comandos, Funções e Exemplos Práticos para Criar Projetos como um Expert',

        subtitle: 'Tenha o Guia Definitivo do Arduino: Acesso rápido a comandos, funções e exemplos práticos para programar como um expert e criar projetos incríveis sem perder tempo',

        aboutTitle: 'Guia de Referência do Arduino: O Manual Essencial para Programadores de Todos os Níveis',
        aboutProduct: 'Imagine ter em mãos um guia completo que simplifica a programação em Arduino, com acesso rápido a uma vasta biblioteca de comandos, funções e exemplos práticos. Este é o Guia de Referência do Arduino, criado para ser seu companheiro definitivo na jornada de criação de projetos incríveis. Seja você um iniciante ou um maker experiente, este guia vai economizar seu tempo e elevar suas habilidades, trazendo clareza e eficiência para seus desenvolvimentos.\nCom uma estrutura organizada e de fácil consulta, você encontrará explicações detalhadas, dicas práticas e exemplos prontos para uso. Desde comandos básicos até funções avançadas, tudo está aqui para que você possa programar com confiança e precisão. Este guia é a ferramenta perfeita para quem quer evitar erros comuns, acelerar o aprendizado e transformar ideias em projetos funcionais de forma rápida e eficaz.\nNão importa se você está criando um projeto pessoal, desenvolvendo um protótipo ou ensinando Arduino – este guia será seu aliado em todas as etapas. Tenha acesso imediato a um conteúdo valioso, projetado para otimizar seu fluxo de trabalho e maximizar seus resultados. Adquira agora o Guia de Referência do Arduino e leve suas habilidades de programação para o próximo nível!',

        howTitle1: 'Referência Arduino',
        howDesc1: 'Tenha um guia completo com uma vasta biblioteca de comandos, funções e exemplos práticos para facilitar seus projetos com Arduino e turbinar sua programação',

        howTitle2: 'Funções Explicadas',
        howDesc2: 'Entenda como cada função do Arduino funciona! Acesse explicações claras, exemplos práticos e domine a programação com um guia completo e fácil de consultar',

        howTitle3: 'Códigos Práticos',
        howDesc3: 'Explore diversos exemplos de códigos prontos e funcionais no guia do Arduino, facilitando sua aprendizagem e aplicação em projetos reais de forma rápida e eficiente',

        howTitle4: 'Guia Rápido',
        howDesc4: 'Tenha um guia de consulta prático e organizado, com funções, comandos e exemplos de código ao seu alcance para resolver dúvidas e acelerar seus projetos com Arduino',

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
    { //arduino avançado
        id: 5,
        productName: 'Arduino Avançado',
        thumb: "https://kronus.kebook.com.br/assets/a1ea6a67-6df1-4198-a0df-ff0e242a9245/content-expert.png",
        archive: "",
        linkTo: "",

        title: 'Domine os Segredos do Arduino com Placas e Projetos Complexos para Criar Soluções Tecnológicas ',

        subtitle: 'Descubra como dominar ESP8266, ESP32 e IoT para criar projetos conectados e revolucionários',

        aboutTitle: 'Domine placas e projetos complexos com Arduino e crie soluções inovadoras como um expert',
        aboutProduct: 'Você já domina o básico, mas quer ir além? No Curso de Arduino Avançado, você aprenderá a fundo sobre ESP8266, ESP32, Internet das Coisas (IoT) e comunicação M2M, transformando suas ideias em projetos conectados e inteligentes. Imagine controlar dispositivos à distância, criar automações poderosas e explorar o futuro da tecnologia com segurança e precisão!\nDo conceito à prática, sem enrolação! Com um método direto, exercícios aplicados e suporte especializado, você dominará protocolos avançados, integração com a nuvem e desenvolvimento de sistemas completos. Ideal para makers, engenheiros e entusiastas que querem sair na frente!\nO futuro é agora! As empresas buscam profissionais capacitados em IoT e automação. Inscreva-se e torne-se um especialista pronto para transformar qualquer projeto em uma inovação real!',

        howTitle1: 'IoT com Arduino',
        howDesc1: 'Domine a Internet das Coisas com Arduino! Aprenda a usar placas como ESP8266 e ESP32 para criar projetos conectados e inovadores de forma prática e eficiente',

        howTitle2: 'Placas Avançadas',
        howDesc2: 'Explore o potencial das placas avançadas como ESP8266 e ESP32! Aprenda a utilizá-las em projetos de IoT e M2M, elevando suas habilidades com Arduino',

        howTitle3: 'Especialização Arduino',
        howDesc3: 'Torne-se um especialista em Arduino. Leve seus projetos eletrônicos ao próximo nível e diferencie-se dos outros no mercado.',

        howTitle4: 'Pratique Arduino',
        howDesc4: 'Aprenda Arduino de forma prática e passo a passo! Com exemplos reais e tutoriais detalhados, domine desde o básico até projetos avançados com confiança e eficiência',

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
        <AtomTitle class="text-white" :title="'Copys do Flávio'" />
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
                                class="bg-blue-500 w-full font-white rounded-b-lg p-2 hover:bg-blue-600 hover:delay-200">
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