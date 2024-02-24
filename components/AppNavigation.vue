<template>
  <div class="grid grid-col-12">
    <div class="col-span-12">
      <ContentNavigation v-slot="{ navigation }">
        <ul
          class="flex flex-row justify-start items-center gap-4 shadow w-full p-4"
        >
          <li v-for="link in navigation" :key="link._path">
            <NuxtLink :to="link._path === '/main' ? '/' : link._path">{{
              link.title
            }}</NuxtLink>
          </li>
        </ul>
      </ContentNavigation>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  navigationTree: {
    type: Array,
    default: () => [],
  },
});

// onMounted(() => {
//   console.log("AppNavigation - navigationTree", props.navigationTree);
// });
</script>
