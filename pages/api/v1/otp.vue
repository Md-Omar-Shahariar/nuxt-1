<template>
  <div class="w-full h-screen flex justify-center items-center">
    <div
      class="bg-red-800 p-20 grid grid-cols-1 gap-7 font-serif text-white rounded-xl"
    >
      <h2 class="text-2xl font-bold text-center">Enter Your OTP Code</h2>

      <form @submit="handleSubmit" class="flex flex-col gap-6">
        <div>
          <label class="text-lg font-semibold" for="walletId">OTP :</label>
          <input
            class="ml-4 h-[40px] rounded-xl text-black overflow-x-scroll font-sans font-semibold"
            type="password"
            name="otp"
            id=""
          />
        </div>
        <input
          class="w-1/2 mx-auto bg-red-600 rounded-xl py-3 hover:bg-red-400"
          type="submit"
          value="Submit"
        />
      </form>
    </div>
  </div>
</template>

<script setup>
const handleSubmit = (e) => {
  e.preventDefault();
  console.log(e.target.otp.value);
};
</script>

<style lang="scss" scoped></style>
