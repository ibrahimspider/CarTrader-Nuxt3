<template>
    <div class="mt-32 flex">
        <!-- CAR SIDE BAR -->
        <CarSideBar />
        <!-- CAR CARDS -->
        <NuxtPage />
    </div>
</template>

<script setup>
const route = useRoute();
const { toTitleCase } = useUtilities();

useHead({
    title: `${route.params.make ? toTitleCase(route.params.make) : 'Cars'} In ${toTitleCase(route.params.city)}`
});
definePageMeta({
    layout: 'custom'
});
</script>

