<template>
  <div>
    <h1>Привет это продукты</h1>
  </div>
</template>
<script>

export default {
data: function(){
    products
},
methods:{
 async asyncData({ $axios, globalPage }) {
    const photo = await $axios.$get(
      `https://api.pexels.com/v1/curated?page=${globalPage}&per_page=24`,
      {
        method: 'GET',
        headers: {
          Authorization:
          key.KEY
        },
      }
}
}
</script>

<style lang="">

</style>
