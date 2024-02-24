<template>
  <div>
    <NuxtLayout name="base">
      <MainBlock />
    </NuxtLayout>
  </div>
</template>

<script lang="ts" setup>
useHead({
  script: [{ src: "./../public/admin/netlify-identity-widget.js" }],
});
</script>
