<template>
  <nav class="...">
    <li v-for="i in items" :key="i">{{ i }}</li>
  </nav>
</template>

<script>
export default {
  name: "HorizontalMenu",
  data() {
    return { items: ["item 1", "item 2", "item 3", "item 4"] };
  },
};
</script>
