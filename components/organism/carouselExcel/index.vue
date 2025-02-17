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
    {//Quero Aprender Dashboard
        id: 2,
        productName: 'Aula: Como Criar um Dashboard',
        thumb: "https://kronus.kebook.com.br/assets/c6aa3ce7-c296-43a4-bc75-1b21b95d4b5a/content-expert.png",
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
    {//Aula: Tudo sobre Função SE
        id: 3,
        productName: 'Aula: Tudo sobre Função SE',
        thumb: "https://kronus.kebook.com.br/assets/a6f95149-ab00-49be-9d75-5690a4581d20/content-expert.png",
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