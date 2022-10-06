<template>
    <div class="border mx-1 bg-light   my-2 px-3 py-4" >
        <h5 class="text-center"> {{menu.title}}</h5>
        <p >{{menu.desc}}{{menu.desc}}{{menu.desc}}{{menu.desc}}</p>
        <p >{{menu.desc}}{{menu.desc}}{{menu.desc}}{{menu.desc}}</p>
        <p >{{menu.desc}}{{menu.desc}}{{menu.desc}}{{menu.desc}}</p>

      </div>
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