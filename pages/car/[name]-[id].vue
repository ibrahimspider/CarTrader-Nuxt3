<template>
    <!-- CAR HERO -->
    <CarDetailHero />
    <!-- CAR ATTRIBUTES -->
    <CarDetailAttributes />
    <!-- CAR DESCRISPTION -->
    <CarDetailDescrisption />
    <!-- CAR CONTACT -->
    <CarDetailContact />
</template>

<script setup>
const route = useRoute();
const { toTitleCase } = useUtilities();

useHead({
    title: `Car ${toTitleCase(route.params.name)}`
});

definePageMeta({
    layout: 'custom'
});
</script>