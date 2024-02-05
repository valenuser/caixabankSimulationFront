<template>
    <section class="w-[100%] h-[100vh] flex flex-col items-center bg-[#008ECF]">
        <div class="w-[100%] h-[30vh] flex items-center justify-center">
            <h1 class="font-bold text-[50px] text-white">CaixaBank</h1>
            <img src="https://i0.wp.com/bankflip.io/wp-content/uploads/2022/01/Caixabank-logo.png?resize=512%2C512&ssl=1" alt="" class="w-[60px] ml-2">
            
        </div>
        <div class="bg-[#008ECF] w-[100%] h-[90vh]">
            <div class="flex flex-col items-center justify-around bg-[#008ECF] w-[100%] h-[50vh]">
                <p class="text-white text-4xl">Buenas noches</p>
                <div class="flex items-center justify-around w-[80%]">
                    <i class="fa-solid fa-user text-[25px] text-white mr-5"></i>
                    <input type="text" placeholder="Username" class="border-b-2 border-white outline-none w-[300px] text-white bg-transparent placeholder-white" maxlength="10">
                </div>
                <div class="flex items-center justify-around w-[80%]">
                    <i class="fa-solid fa-lock text-[25px] text-white mr-5"></i>
                    <input type="password" placeholder="Password" class="border-b-2 border-white outline-none w-[300px] text-white bg-transparent placeholder-white" maxlength="10">
                </div>
                <button class="bg-white w-[150px] h-[35px] rounded text-cyan-600 font-bold" @click="login">Entrar</button>
            </div>
            <div class="w-[100%] h-[20vh] flex flex-col items-center justify-center bg-[#008ECF]">
                <p class="text-gray-300">¿No estas registrado?</p>
                <router-link to="register" class="text-white">Resgistrarse</router-link>
            </div>
        </div>
    </section>
</template>
<script>
export default{
    methods:{
        login(){
            this.$router.push({name:'main'})
        }
    }
}
</script>