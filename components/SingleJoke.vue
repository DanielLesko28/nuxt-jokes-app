<template>
  <nuxt-link :to="'jokes/' + id">
    <div class="p-4 border-2 border-dotted my-4">
      <p>{{ joke }}</p>
    </div>
  </nuxt-link>
</template>

<script>
export default {
    name: 'SingleJoke',
    props:{
        joke:{
            type: String,
            default: ''
        },
        id:{
            type: String,
            default: ''
        },
    }
}
</script>

<style>

</style>