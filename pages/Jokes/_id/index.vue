<template>
  <div class="w-full">
    <nuxt-link to="/jokes" class="bg-red-400 p-2 rounded-lg m-4 text-white">Back To Jokes</nuxt-link>
    <h2 class="font-bold my-4 self-center">{{ joke }}</h2>
    <hr />
    <small>Joke ID: {{ $route.params.id }}</small>
  </div>
</template>

<script>
import axios from 'axios'
export default {
    data(){
        return{
            joke:{}
        }
    },
    async created(){
        const config = {
            headers: {
                'Accept': 'application/json'
            }
        }

        try{
            const res = await axios.get(`https://icanhazdadjoke.com/j/${this.$route.params.id}`, config);
            this.joke = res.data.joke;
        } catch (err){
            console.log(err);
        }
    }
}
</script>

<style>

</style>