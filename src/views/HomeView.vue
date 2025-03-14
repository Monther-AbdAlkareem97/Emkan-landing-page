<template>
  <div>
    <navBarComponent />
    <aboutUsComponent />
    <servicesComponent />
    <whyUsComponent />
    <footerComponent />

    <button
      v-show="showScrollTop"
      @click="scrollToTop"
      class="w-14 h-14 fixed bottom-40 right-5 bg-slate-800 text-white p-3 rounded-full transition duration-300 hover:bg-slate-900 hover:scale-110"
    >
      <font-awesome-icon icon="arrow-up" class="text-2xl" />
    </button>
  </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";
import navBarComponent from "@/components/navBarComponent.vue";
import aboutUsComponent from "@/components/aboutUsComponent.vue";
import servicesComponent from "@/components/servicesComponent.vue";
import whyUsComponent from "@/components/whyUsComponent.vue";
import footerComponent from "@/components/footerComponent.vue";

const showScrollTop = ref(false);

const handleScroll = () => {
  showScrollTop.value = window.scrollY > 200;
};

const scrollToTop = () => {
  window.scrollTo({ top: 0, behavior: "smooth" });
};

onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});

onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>

<style scoped></style>
