<template>
    <b-container fluid>
      <NavBar></NavBar>
      <b-row align-h="center mx-3">
        <b-col class="text-center my-4" cols="12">
          <h3>Our Menu</h3>
        </b-col>
        <b-col v-for="menu in menus" :key="menu.title" lg="4" md="5" sm="12" xs="12">
          <Card :menu="menu"></Card>
        </b-col>
      </b-row> 
    </b-container>
</template>

<script>
import Card from '@/components/Card.vue'
import NavBar from '@/components/NavBar.vue';
const lorem = `
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. 
    `;
export default {
  name: 'App',
  components: { Card, NavBar },
  data () {
  return {
  
    menus: [
      {
        title: "Chicken",
        desc: lorem
      },
      {
        title: "Beef",
        desc: lorem
      },
      {
        title: "Sushi",
        desc: lorem
      }
    ]
  }
 }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
