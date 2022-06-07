<template>
  <div class="flex flex-col h-screen justify-between">
    <Header class="fixed-top"></Header>
    <div id="main" class="w-full" ></div>
    <Footer class="w-full"></Footer>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>

<style>
#main{
  background: linear-gradient(to bottom, #222126dc, #393d42dc), url('../assets/img/pexels-tiger-lily-4483610.jpeg');
  background-size: cover;
  height: 80vh;
}
</style>