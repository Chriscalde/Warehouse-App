<template>
  <div class="flex flex-col bg-gray-100">
    <Header></Header>
    <div class="m-32 rounded-xl shadow-2xl flex flex-col bg-white">
        <h1 class="text-center text-2xl text-gray-800 mt-4">Welcome, User</h1>
        <div class="grid grid-cols-3 gap-12 justify-center p-16">
            <div class="rounded-2xl bg-green-200 text-center text-2xl text-gray-800 flex flex-col p-4">
                <i class="bx bx-notepad text-3xl"></i>
                <a href="/jobs">Jobs</a>
            </div>
            <div class="rounded-2xl bg-green-200 text-center text-2xl text-gray-800 flex flex-col p-4">
                <i class="bx bx-user text-3xl"></i>
                <a href="">Installers</a>
            </div>
            <div class="rounded-2xl bg-green-200 text-center text-2xl text-gray-800 flex flex-col p-4">
                <i class="bx bx-cube text-3xl"></i>
                <a href="">Inventory</a>
            </div>
        </div>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
export default {
    name:'DashboardPage'
}
</script>

<style>

</style>