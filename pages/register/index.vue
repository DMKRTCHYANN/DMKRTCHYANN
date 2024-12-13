<template>
  <div class="flex  items-center">
    <div class="w-full  flex justify-center">
      <div>
          <h1 class="flex text-3xl font-extrabold  mb-6">Get Started Now</h1>
          <div class="space-y-4">
            <div>
              <p>Name</p>
              <custom-input @input="onHover($event)"></custom-input>
              <!--            <input class="w-full p-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-[#3A5B22]" type="text" placeholder="Enter your name"/>-->
            </div>
            <div>
              <p>Email address</p>
              <input class="w-full p-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-[#3A5B22]" type="email" placeholder="Enter your email"/>
            </div>
            <div>
              <p>Password</p>
              <input  class="w-full p-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-[#3A5B22]" type="password" placeholder="Create password"/>
            </div>
            <input type="checkbox" id="a">
             <label for="a">I agree to the terms & polity</label>
            <button class="w-full rounded-[10px]  bg-[#3A5B22] font-bold  text-white px-4 py-2 cursor-pointer" type="submit">
              Register
            </button>
            <div class="flex space-x-4 items-center justify-center">
              <button class="flex items-center space-x-2 rounded-[20px] px-4 py-2 border border-seri  cursor-pointer">
                <img src="/images/icons8-apple-logo%201.png" alt="Google Icon" class="h-6 w-6"/>
                <span>Sign in with Google</span>
              </button>
              <button class="flex items-center space-x-2 rounded-[20px] px-4 py-2 border border-seri   cursor-pointer">
                <img src="/images/icons8-apple-logo%201.png" alt="Apple Icon" class="h-6 w-6"/>
                <span>Sign in with Apple</span>
              </button>
            </div>
            <div class="text-center">
              <p>Have an account? Sign in</p>
            </div>
          </div>
      </div>
    </div>
      <img class="w-full h-[960px]" src="/images/login_bg.png" alt=""/>
  </div>
</template>
<script setup>
import CustomInput from "~/components/CustomInput.vue";
</script>