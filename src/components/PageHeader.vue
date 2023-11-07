<template>
  <div class="flex justify-between bg-purple-200 px-6 py-4">
    <div class="text-xl font-semi-bold">Sites'R'Us</div>
    <HorizontalMenu />
  </div>
</template>
<script>
import HorizontalMenu from "./HorizontalMenu.vue";

export default { name: "PageHeader", components: { HorizontalMenu } };
</script>
