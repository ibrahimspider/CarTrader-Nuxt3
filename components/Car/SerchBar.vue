<template>
    <div
        class=" max-w-[1000px] text-2xl rounded-md flex justify-between overflow-hidden shadow-2xl mx-auto">
        <input type="text" class="py-3 px-5 w-full text-2xl rounded-l-md focus:outline-none border-2" v-model="city"
            placeholder="Search by city..." :class="citError ? 'border-red-500 ' : ''" />
        <button class="bg-gray-700 px-5 text-white" @click="handleSerch">Search</button>
    </div>
</template>

<script setup>
const city = ref("");
const citError = ref(false)

const handleSerch = () => {
    if (!city.value) {
        return citError.value = true
    }
    navigateTo(`/city/${city.value}/car`)
}
</script>