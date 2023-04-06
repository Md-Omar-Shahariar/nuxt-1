<template>
  <div>
    <div class="w-full bg-[#00763A]">
      <nav
        class="h-[70px] container mx-auto flex items-center justify-between text-white font-sans"
      >
        <div class=""><p class="font-bold text-xl">FSIBL</p></div>

        <ul class="flex h-full text-lg">
          <div class="h-full flex hover:bg-[#13442b]">
            <li class="my-auto px-2">
              <NuxtLink to="/api/v1">Home</NuxtLink>
            </li>
          </div>
          <div class="h-full flex hover:bg-[#13442b]">
            <li class="my-auto px-2">
              <NuxtLink to="/api/v1/otp">About Us</NuxtLink>
            </li>
          </div>
          <div class="h-full flex hover:bg-[#13442b]">
            <li class="my-auto px-2">
              <NuxtLink to="/api/v1/form">Contact Us</NuxtLink>
            </li>
          </div>
          <div class="h-full flex hover:bg-[#13442b]">
            <li class="my-auto px-2">
              <NuxtLink to="/api/v1">Log out</NuxtLink>
            </li>
          </div>
        </ul>
      </nav>
    </div>
    <div class="container grid grid-cols-5">
      <div class="col-span-1 shadow-2xl">
        <div class="my-4 flex flex-col items-center">
          <img
            class="bg-white rounded-full h-[100px] w-[100px]"
            src="../assets/images/icons/user2.jpg"
            alt=""
          />
          <p class=""><span class="text-xl font-sans">User</span></p>
        </div>
        <hr />
        <div class="py-3">
          <NuxtLink class="block text-center">Manage Account</NuxtLink>
        </div>
        <hr />
        <div class="py-3">
          <NuxtLink class="block text-center">demo Link</NuxtLink>
        </div>
        <hr />
        <div class="py-3">
          <NuxtLink class="block text-center">demo Link</NuxtLink>
        </div>
        <hr />
        <div class="py-3">
          <NuxtLink class="block text-center">demo Link</NuxtLink>
        </div>
        <hr />
      </div>
      <slot />
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
