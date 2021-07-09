<template>
  <div class="home">
    <!-- hardcoding story here until I determine how to store in a database or some other method. -->
    <!-- potential recurring component setup here -->
    <h2 class="title">Chapter 1: The Beginning</h2>
    <p class="story">
      I will never forget February, 2021. My wife and I were working from home
      in a house we've been renting for nearly 5 years. Around noon, we received
      a call from the rental company telling us the owner was looking to sell
      the house and we needed to leave within 30 days. Of course, this set off a
      panic for both of us because, as anyone who moves will tell you, we knew
      it was going to be hard to find a new place, it would be expensive, and we
      would have to coordinate with work to figure out what to do.
    </p>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
// import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src

@Component<HomePage>({
  components: {},
})
export default class HomePage extends Vue {}
</script>

<style scoped lang="scss">
.title {
  text-decoration: underline;
  font-weight: bold;
  margin-bottom: 2em;
}
.story {
  text-align: left;
  text-indent: 2em;
}
</style>
