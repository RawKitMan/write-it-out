<template>
  <div>
    <b-navbar toggleable="lg" type="light">
      <b-navbar-brand href="#">Our Journey</b-navbar-brand>
      <b-navbar-toggle target="hamburger" />

      <b-collapse id="hamburger" is-nav>
        <b-navbar-nav>
          <b-nav-item to="/">Home</b-nav-item>
          <b-nav-item to="/archive">Archive</b-nav-item>
          <b-nav-item to="/about">About</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script lang="ts">
/* eslint-disable */
import Vue from "vue";
import Component from "vue-class-component";

@Component<Header>({})
export default class Header extends Vue {}
</script>

<style scoped lang="scss">
.navbar {
  @include setBorder();
  border-top: 0;
  border-left: 0;
  border-right: 0;
  margin-bottom: 10px;
  background-color: $colorLightTan;
  color: $colorDarkGreen;
  font-weight: bold;
}
</style>
