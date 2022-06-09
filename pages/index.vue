<template>
  <div class="flex flex-col h-screen justify-between">
    <Header class=""></Header>
    <div id="main" class="w-full" >
      <section id="welcome">
        <div class="grid grid-cols-2 gap-2 bg-white rounded-xl m-12">
          <div id="welcome-first" class="text-center p-20">
            <h1 class="text-6xl mb-10">Hello There!</h1>
            <p class="text-xl">Welcome to the Warehouse Application</p>
            <p class="text-xl mb-6">Please, login to continue</p>
            <button class="bg-green-400 rounded-2xl text-2xl text-white py-2 px-6">Login</button>
          </div>
          <div id="welcome-second" class="grid grid-cols-3 text-center align-middle items-center justify-center text-4xl bg-green-400 rounded m-4">
            <div>
              <h1>Orders</h1>
              <i class="bx bx-book-content"></i>
            </div>
            <div>
              <h1>Installers</h1>
              <i class="bx bx-user-pin"></i>
            </div>
            <div>
              <h1>Jobs</h1>
              <i class="bx bx-buildings"></i>
            </div>
          </div>
        </div>
      </section>
    </div>
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