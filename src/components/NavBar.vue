<template>
    <b-navbar toggleable="lg" >
      <b-navbar-brand to="/">
        <a class="navbar-brand mx-3" href="#">Food, LLC</a>
      </b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav />
        <b-navbar-nav align="right" class="d-sm-block d-md-none">
          <b-nav-item v-for="nav in navItems" class="text-center" :key="nav">
            <b-button variant="text-secondary">{{nav}}</b-button>
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>

    </b-navbar>
</template>

<script>
export default {
  data() {
    return {
      navItems: ["Chicken", "Beef", "Sushi"]
    };
  }
};
</script>

<style>
</style>