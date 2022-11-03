<template>
  <div class="w-full text-center">
    <h1 class="font-bold text-2xl">About Jokes</h1>
    <p class="font-medium text-lg">I made this app for anyone who wants to laugh</p>
  </div>
</template>

<script>
export default {
    head(){
        return {
            title: 'About',
            meta: [
                {
                    hid: 'description',
                    name: 'description',
                    content: 'Best place for jokes'
                }
            ]
        };
    }
};
</script>

<style>

</style>