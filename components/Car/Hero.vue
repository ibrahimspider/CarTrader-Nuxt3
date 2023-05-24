<template>
    <div
        class="relative h-screen w-100 bg-no-repeat bg-cover bg-bottom bg-[url('https://carconfigurator.ferrari.com/assets/cars/portofinom/packages/default/car-ferrari-portofino-m_splash.jpg')]">
        <div class="z-10 absolute w-full h-full flex justify-center items-center bg-[rgba(0,0,0,0.5)]">
            <div class="text-center w-[80%]">
                <h1 class="text-5xl  mb-10 text-white font-bold leading-snug">Find your drive</h1>
                <!-- HOME SEARCH BAR -->
                <CarSerchBar />
                <!-- HOME SEARCH BAR -->
            </div>
        </div>
        <div class="z-1 absolute w-full h-full bg-black opacity-50"></div>
    </div>
</template>

<script>
export default {

}
</script>