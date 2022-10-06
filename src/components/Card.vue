<template>
  <b-container>
    <div class="border py-3 mx-1 bg-secondary   my-2 px-2 py-2" >
        <h5 class="text-center"> {{menu.title}}</h5>
        <p >{{menu.desc}}{{menu.desc}}{{menu.desc}}{{menu.desc}}</p>
        <p >{{menu.desc}}{{menu.desc}}{{menu.desc}}{{menu.desc}}</p>
      </div>
  </b-container>
</template>

<script>
export default {
  props: {
    menu: {
        type: Object,
        required: true
    }
  }
}
</script>

<style>

</style>