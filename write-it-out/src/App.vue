<template>
  <div id="app">
    <Header />
    <BContainer id="container">
      <main class="main">
        <router-view />
      </main>
    </BContainer>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Header from "@/components/Layout/Header.vue";
import { BContainer } from "bootstrap-vue";

@Component<App>({
  components: {
    Header,
    BContainer,
  },
})
export default class App extends Vue {}
</script>

<style scoped lang="scss"></style>
