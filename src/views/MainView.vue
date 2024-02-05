<template>
    <section class="w-[100%] h-[100vh] flex flex-col items-center">
        <div class="w-[100%] h-[25vh] flex  flex-col items-center justify-center overflow-hidden">
            <div class="z-20 absolute w-[100%] h-[40px]  top-0 right-0  flex items-center justify-end">
                <div class="bg-white w-[35px] h-[35px] rounded-[100%] mr-2 flex items-center justify-center">
                    <p class="text-[20px] font-bold">V</p>
                </div>
            </div>
            <div class="z-10 border absolute w-[200px] h-[70px] mt-5 rounded bg-white flex items-center flex-col  justify-center">
                <p class="text-gray-500">ES12 3456 7890 1234</p>
                <p class="text-[30px]">10.000€</p>
            </div>
            <div class="bg-[#008ECF] w-[100%] h-[70vh] z-0"></div>
            <div class=" w-[100%] h-[55vh] z-0 "></div>
        </div>
        <div class="w-[100%] h-[65vh]  flex flex-col justify-around">
            <div class="flex flex-col">
                <h1 class="font-bold">Ultimos bizums enviados:</h1>
                <div class="w-[100%] h-[20vh] flex flex-col items-center justify-around">
                    <div class="flex justify-around border w-[350px] h-[50px] items-center rounded">
                        <p class="text-[18px] ">01/01/24</p>
                        <p class="text-[18px] ">Compra mercadona</p>
                        <p class="text-[18px] font-bold text-red-500">-200€</p>
                    </div>
                    <div class="flex justify-around border w-[350px] h-[50px] items-center rounded">
                        <p class="text-[18px] ">01/01/24</p>
                        <p class="text-[18px] ">Entrada futbol</p>
                        <p class="text-[18px] font-bold text-red-500">-50€</p>
                    </div>
                </div>
            </div>
            <div class="flex flex-col">
                <h1 class="font-bold">Ultimos bizums recibidos:</h1>
                <div class="w-[100%] h-[20vh] flex flex-col items-center justify-around">
                    <div class="flex justify-around border w-[350px] h-[50px] items-center rounded">
                        <p class="text-[18px] ">01/01/24</p>
                        <p class="text-[18px] ">Doble paga</p>
                        <p class="text-[18px] font-bold text-green-500">+900€</p>
                    </div>
                    <div class="flex justify-around border w-[350px] h-[50px] items-center rounded">
                        <p class="text-[18px] ">01/01/24</p>
                        <p class="text-[18px] ">Cena empresa</p>
                        <p class="text-[18px] font-bold text-green-500">+200€</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="w-[100%] h-[10vh] flex justify-around border items-center">
            <i class="fa-solid fa-list text-[30px]"></i>
            <img src="https://femivoz.es/wp-content/uploads/logo-bizum-v2.png" alt="" class="w-[50px]">
            <i class="fa-solid fa-arrow-right-from-bracket text-[30px]" @click="logout"></i>
        </div>
    </section>
</template>
<script>
export default{
    methods:{
        logout(){
            this.$router.push({name:'home'})
        }
    }
}
</script>