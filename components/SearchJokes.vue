<template>
  <form class="flex justify-center" @submit.prevent="onSubmit">
    <input v-model="text" class="mx-2 px-2" type="text" placeholder="Search Jokes..." />
    <input class="border-2 p-2 rounded-md bg-red-500 text-white" type="submit" value="Search Jokes" />
  </form>
</template>

<script>
export default {
    name: 'SearchJokes',
    data(){
        return{
            text: ''
        }
    },
    methods:{
        onSubmit(){
            this.$emit('search-text', this.text)
            this.text = ''
        }
    }
}
</script>

<style>

</style>