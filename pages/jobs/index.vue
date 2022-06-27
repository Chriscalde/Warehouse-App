<template>
  <div class="flex flex-col bg-gray-300">
    <Header></Header>
    <div class="m-32 bg-gray-200 rounded-2xl shadow-2xl grid grid-cols-5">
        <div class="bg-gray-100 rounded-2xl flex flex-col p-2">
            <h1 class="text-2xl text-gray-800 my-8 text-center">Jobs</h1>
            <a class="text-xl my-4 p-2 bg-green-400 rounded text-white inline-flex items-center" href=""><i class="bx bx-notepad mr-4"></i>Jobs</a>
            <a class="text-xl my-4 p-2 rounded hover:bg-green-100 inline-flex items-center" href=""><i class="bx bx-user mr-4"></i>Installers</a>
            <a class="text-xl my-4 p-2 rounded hover:bg-green-100 inline-flex items-center" href=""><i class="bx bx-cube mr-4"></i>Inventory</a>
        </div>
        <div class="col-span-4 flex flex-col m-12">
            <div class="ml-auto">
            <input type="text" class="bg-gray-100 rounded-md p-2 border-green-400 focus:ring focus:border-green-400 focus:ring-green-400" placeholder="Search...">
            </div>
            <div class="flex flex-wrap mt-8">
                <a href="" class="mr-auto text-3xl">Jobs</a>
                <div class="grid grid-cols-2 gap-8">
                    <button class="bg-white rounded-2xl px-4 py-2 inline-flex items-center"><i class="bx bx-filter-alt text-2xl mr-2"></i> Filters</button>    
                    <button class="bg-green-400 rounded-2xl px-4 py-2 text-white inline-flex items-center"><i class="bx bx-plus text-2xl mr-2"></i> New Job</button>    
                </div>
            </div>
        </div>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
export default {
    name:'JobsPage'
}
</script>

<style>
    .class-left{
        background-color: green !important;
        background-size: cover;
    }

    input:focus{
        outline: none !important;
    }
</style>