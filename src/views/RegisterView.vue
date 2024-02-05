<template>
    <section class="w-[100%] h-[100vh] flex flex-col items-center bg-[#008ECF]">
        <img src="https://cdn6.aptoide.com/imgs/4/7/3/4739d1f61593c25ced217c066103c6d9_screen.jpg" alt="" class="w-[100%] h-[30vh]">
        <div class="bg-cyan-600 w-[100%] h-[90vh]">
            <div class="flex flex-col items-center justify-around bg-[#008ECF] w-[100%] h-[50vh]">
                <p class="text-white text-4xl">Register</p>
                <input type="text" placeholder="Username" class="border-b-2 border-white outline-none w-[300px] text-white bg-transparent placeholder-white" maxlength="10">
                <input type="text" placeholder="Password" class="border-b-2 border-white outline-none w-[300px] text-white bg-transparent placeholder-white" maxlength="10">
                <button class="bg-white w-[150px] h-[35px] rounded text-[#008ECF] font-bold">Registrarse</button>
            </div>
            <div class="w-[100%] h-[20vh] flex flex-col items-center justify-center bg-[#008ECF]">
                <p class="text-gray-300">Ya estas registrado?</p>
                <router-link to="/" class="text-white">Iniciar sesion</router-link>
            </div>
        </div>
    </section>
</template>