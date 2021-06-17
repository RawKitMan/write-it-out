<template>
    <div>
        <b-navbar toggleable="lg" type="light" variant="primary">
            <b-navbar-brand href="#">Write It Out</b-navbar-brand>
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
import Vue from 'vue';
import Component from 'vue-class-component';

@Component<Header>({

})
export default class Header extends Vue{
}
</script>

<style scoped>

</style>
