<template>
  <div class="flex flex-col bg-gray-300">
    <Header></Header>
    <div class="container-jobs m-32 bg-gray-200 rounded-2xl shadow-2xl grid grid-cols-5">
        <div class="bg-gray-100 rounded-2xl flex flex-col p-2">
            <h1 class="text-2xl text-gray-800 my-8 text-center">Installers</h1>
            <a class="text-xl my-4 p-2 rounded hover:bg-green-50  inline-flex items-center" href="/jobs"><i class="bx bx-notepad mr-4"></i>Jobs</a>
            <a class="text-xl my-4 p-2 bg-green-400 hover:bg-green-500 rounded text-white inline-flex items-center" href="/installers"><i class="bx bx-user mr-4"></i>Installers</a>
            <a class="text-xl my-4 p-2 rounded hover:bg-green-50 inline-flex items-center" href=""><i class="bx bx-cube mr-4"></i>Inventory</a>
        </div>
        <div class="col-span-4 flex flex-col m-12">
            <div class="ml-auto">
            <input type="text" class="bg-gray-100 rounded-md p-2 border-green-400 focus:ring focus:border-green-400 focus:ring-green-400" placeholder="Search...">
            </div>
            <div class="flex flex-wrap mt-8">
                <a href="" class="mr-auto text-3xl">Installers</a>
                <div class="grid grid-cols-2 gap-8">
                    <button class="bg-white rounded-2xl px-4 py-2 inline-flex items-center"><i class="bx bx-filter-alt text-2xl mr-2"></i> Filters</button>    
                    <button class="bg-green-400 rounded-2xl px-4 py-2 text-white inline-flex items-center"><i class="bx bx-plus text-2xl mr-2"></i> New Installer</button>    
                </div>
            </div>
            <div class="flex">
                <table class="table-fixed w-full border-separate p-4 text-center">
                    <thead>
                        <tr>
                            <th class="w-1/3">Name</th>
                            <th class="w-1/3">Phone</th>
                            <th class="w-1/6">Options</th>
                            <th class="w-1/6"></th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr class="my-4">
                            <td>John Doe</td>
                            <td>+1 234 567 89 01</td>
                            <td class="hover:bg-green-500 rounded-xl text-white bg-green-400">Assign New</td>
                            <td class="hover:text-red-600 inline-flex items-center text-red-500"><i class="text-2xl  bx bxs-x-circle"></i></td>
                        </tr>
                        <tr class="my-4">
                            <td>John Doe</td>
                            <td>+1 234 567 89 01</td>
                            <td class="hover:bg-green-500 rounded-xl text-white bg-green-400">Assign New</td>
                            <td class="hover:text-red-600 inline-flex items-center text-red-500"><i class="text-2xl bx bxs-x-circle"></i></td>
                        </tr>
                        <tr class="my-4">
                            <td>John Doe</td>
                            <td>+1 234 567 89 01</td>
                            <td class="hover:bg-green-500 rounded-xl text-white bg-green-400">Assign New</td>
                            <td class="hover:text-red-600 inline-flex items-center text-red-500"><i class="text-2xl bx bxs-x-circle"></i></td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
export default {
    name:'InstallersPage'
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

    .container-jobs{
        min-height: 80% !important;
    }
</style>