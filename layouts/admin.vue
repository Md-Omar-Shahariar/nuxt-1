<template>
  <div>
    <div class="w-full bg-[#00763A]">
      <nav
        class="h-[50px] container mx-auto text-xl flex items-center justify-between"
      >
        <div class=""><p class="font-bold">FSIBL</p></div>
        <div>
          <ul class="flex gap-4">
            <li class=""><NuxtLink to="/api/v1">Home</NuxtLink></li>
            <li><NuxtLink to="/api/v1/otp">About Us</NuxtLink></li>
            <li><NuxtLink to="/api/v1/form">Contact Us</NuxtLink></li>
          </ul>
        </div>
      </nav>
    </div>
    <slot />
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
