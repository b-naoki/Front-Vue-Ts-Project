<template>
  <div class="home">
    <Header />
    <!-- Headerコンポーネントをここに追加 -->
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Header from "@/components/Header.vue"; // Headerをインポート

export default defineComponent({
  name: "HomeView",
  components: {
    Header, // Headerを登録
  },
});
</script>
