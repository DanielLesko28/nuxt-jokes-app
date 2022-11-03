<template>
  <div class="flex flex-col items-center">
    <h1 class="my-2 font-bold text-2xl">Welcome to the best app for jokes</h1>
    <img src="../assets/funnyPicture.jpg" class="w-[700px] rounded-md my-2" alt="some picture" />
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  head(){
        return {
            title: 'Welcome to Jokes',
            meta: [
                {
                    hid: 'description',
                    name: 'description',
                    content: 'Best place for jokes'
                }
            ]
        };
    },
}
</script>
