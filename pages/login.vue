<template>
  <div class="flex flex-col h-screen justify-between">
      <Header></Header>
      <div id="login">
          <section id="login-form">
              <div class="m-24 bg-white rounded-2xl text-center justify-evenly">
                  <h1 class="text-4xl mt-8">Welcome</h1>
                  <div class="p-8 m-12">
                  <form action="" method="post" class="flex flex-col">
                      <label class="block">
                          <span class="text-2xl inline-flex items-center"><i class="bx bx-user mr-2"></i> Username</span>
                          <input type="text" class="bg-gray-200 rounded-md w-48 p-2 ml-6 focus:ring focus:border-green-400 focus:ring-green-400">
                      </label>
                      <label class="block mt-8">
                          <span class="text-2xl inline-flex items-center"><i class="bx bx-key mr-2"></i> Password</span>
                          <input type="text" class="bg-gray-200 rounded-md w-48 p-2 ml-6 focus:ring focus:border-green-400 focus:ring-green-400">
                      </label>
                      <button type="button" class="rounded bg-green-400 text-white text-center text-2xl py-4 px-10 my-8 mx-auto w-auto" @click="loginUser()">Login</button>
                  </form>
                  </div>
              </div>
          </section>
      </div>
      <Footer></Footer>
  </div>
</template>

<script>
export default {
    name: "LoginPage",
    data: () => {
        return{
            username: '',
            password: ''
        }
    },
    methods:{
        loginUser(){
            const user = {
                username: this.username,
                password: this.password
            }
            console.log(user);
            this.$router.push('/dashboard')
            this.$toast.show('Login succesfull',{
                type: 'success',
                icon: 'check',
                duration: 3000
            })
            
        }
    }
}
</script>

<style scoped>
#login{
  background: linear-gradient(to bottom, #222126dc, #393d42dc), url('../assets/img/pexels-tiger-lily-4483610.jpeg');
  background-size: cover;
  height: 80vh;
}

input:focus{
        outline: none !important;
    }
</style>