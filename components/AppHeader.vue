<template>
  <header class="flex justify-between align-center mb-4 pb-4 border-b-2 border-zinc-500">
    <h1 class="text-3xl text-amber-800">Jokes</h1>
    <ul class="flex">
        <li>
            <nuxt-link to="/" class="inline-block bg-black text-white py-2 px-4 mr-2 rounded-md">Home</nuxt-link>
        </li>
        <li>
            <nuxt-link to="/jokes" class="inline-block bg-black text-white py-2 px-4 mr-2 rounded-md">Jokes</nuxt-link>
        </li>
        <li>
            <nuxt-link to="/about" class="inline-block bg-black text-white py-2 px-4 mr-2 rounded-md">About</nuxt-link>
        </li>
    </ul>
  </header>
</template>

<script>
export default {
    name: 'AppHeader',
}
</script>

<style>

</style>