<script setup>
const city = ref("");
const cityError = ref(false);

const handleSearch = () => {
  if (!city.value) {
    return (cityError.value = true);
  }
  navigateTo(`/city/${city.value}/car`);
};
</script>

<template>
  <div
    class="font-serif w-full text-sm md:text-lg lg:text-2xl rounded-full bg-white flex justify-between overflow-hidden drop-shadow-2xl mx-auto"
  >
    <input
      type="text"
      class="py-2 px-5 lg:py-3 lg:px-6 w-full rounded-full focus:outline-none"
      :class="cityError && 'border border-red-500'"
      placeholder="Search by city..."
      v-model="city"
    />
    <button class="bg-sky-500 px-6 md:px-10 text-white" @click="handleSearch">
      Search
    </button>
  </div>
</template>
