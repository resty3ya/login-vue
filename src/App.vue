<script>
import PageHeader from "./components/PageHeader.vue";
import PageFooter from "./components/PageFooter.vue";
import SideMenu from "./components/SideMenu.vue";
import PageContent from "./components/PageContent.vue";
import "tailwindcss/tailwind.css";

export default {
  name: "App",
  components: { PageHeader, PageFooter, SideMenu, PageContent },
};
</script>

<template>
  <div class="container mx-auto">
    <header class="w-full">
      <PageHeader />
    </header>
    <div class="flex space-x-4">
      <div class="w-1/6">
        <SideMenu />
      </div>
      <div class="w-5/6">
        <PageContent />
      </div>
      <footer class="w-full">
        <PageFooter />
      </footer>
    </div>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
