<script setup>
const route = useRoute();

const toTitleCase = (str) => {
  return str.replace(/\w\S*/g, (txt) => {
    return txt.charAt(0).toUpperCase() + txt.substr(1);
  });
};

useHead({
  title: `${route.params.make ? toTitleCase(route.params.make) : "Cars"} in ${toTitleCase(
    route.params.city
  )}`,
});

definePageMeta({
  layout: "custom",
});
</script>

<template>
  <div class="mt-32 flex">
    <CarSideBar />

    <NuxtPage />
  </div>
</template>
