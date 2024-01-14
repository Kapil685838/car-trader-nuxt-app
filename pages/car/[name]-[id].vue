<script setup>
const route = useRoute();

const toTitleCase = (str) => {
  return str.replace(/\w\S*/g, (txt) => {
    return txt.charAt(0).toUpperCase() + txt.substr(1);
  });
};

useHead({
  title: toTitleCase(route.params.name),
});

definePageMeta({
  layout: "custom",
});
</script>

<template>
  <div>
    <CarDetailHero />

    <CarDetailAttributes />

    <CarDetailDescription />

    <CarDetailContact />
  </div>
</template>
