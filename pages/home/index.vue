<template>
  <div>
    <NuxtLayout name="base">
      <HomeBanner />
      <HomeBlock01 />
      <HomeBlock02 />
    </NuxtLayout>
  </div>
</template>

<script lang="ts" setup>
const route = useRoute();

onMounted(() => {
  // console.log("Path", route.path);
  // console.log("name", route.name);
});
</script>
