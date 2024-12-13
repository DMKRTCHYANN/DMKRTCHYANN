<template>
  <div class="flex  items-center">
    <div class="w-full  flex justify-center">
      <div>
        <h1 class="flex text-3xl font-extrabold  mb-6">Welcome back!</h1>
        <p class="flex font-extrabold  mb-6" >Enter your credentials to access your account</p>
        <div class="space-y-4">
          <div>
            <p>Email address</p>
            <custom-input v-model="email"></custom-input>
            {{ email }}
<!--            <input v-model="email" class="w-full p-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-[#3A5B22]"/>-->
          </div>
          <div>
            <div class="flex justify-between">
              <p>Password</p>
              <p class="text-[#0C2A92]">forgot password</p>
            </div>
            <input  class="w-full p-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-[#3A5B22]" type="password" placeholder="Create password"/>
          </div>
          <input type="checkbox" id="a">
          <label for="a">Remember for 30 days </label><br>
          <button class="w-full rounded-[10px]  bg-[#3A5B22] font-bold  text-white px-4 py-2 cursor-pointer" type="submit">
            Login
          </button>
          <div class="flex space-x-4 items-center justify-center">
            <button class="flex items-center space-x-2 rounded-[20px] px-4 py-2 border border-Grey  cursor-pointer">
              <img src="/images/icons8-google%201.png" alt="Google Icon" class="h-6 w-6"/>
              <span>Sign in with Google</span>
            </button>
            <button class="flex items-center space-x-2 rounded-[20px] px-4 py-2 border border-Grey   cursor-pointer">
              <img src="/images/icons8-apple-logo%201.png" alt="Apple Icon" class="h-6 w-6"/>
              <span>Sign in with Apple</span>
            </button>
          </div>
          <div class="text-center">
            <p>Don't Have an account? Sign in</p> {{ email }}
          </div>
        </div>
      </div>
    </div>
    <img class="w-full h-[960px]" src="/images/login_bg.png" alt=""/>
  </div>
</template>
<script setup>

import Aswqdqdwqdwq from "~/components/CustomInput.vue";
import CustomInput from "~/components/CustomInput.vue";

const email = ref('')

</script>