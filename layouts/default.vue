<template>
  <div class="max-w-[1000px] my-8 mx-auto overflow-hidden py-4 px-8 bg-white">
    <AppHeader />
    <Nuxt />
  </div>
</template>

<script>
import AppHeader from '~/components/AppHeader';

export default {
    components:{
        AppHeader
    }
}
</script>

<style>

</style>