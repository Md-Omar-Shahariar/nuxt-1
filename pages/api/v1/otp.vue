<template>
  <div class="w-full h-screen flex justify-center items-center">
    <div
      class="bg-[#00763A] shadow-black shadow-md w-[400px] p-5 grid grid-cols-1 gap-7 font-sans text-white rounded"
    >
      <h2 class="text-2xl font-bold text-center">OTP</h2>
      <form @submit="handleSubmit" class="flex flex-col gap-6">
        <div class="w-full">
          <!-- <label class="text-lg font-semibold" for="walletId">Wallet :</label> -->
          <input
            required
            class="w-full h-[40px] rounded text-black overflow-x-scroll font-sans font-semibold"
            type="text"
            name="otp"
            placeholder=" OTP"
            id=""
          />
        </div>
        <button
          class="w-[100px] flex items-center justify-center h-[40px] content-center ml-auto bg-[#000167] rounded py-3 hover:bg-[#000267a9]"
          type="submit"
        >
          <p class="flex items-center">
            <span>Next</span>
            <img
              class="ml-2 w-[15px] h-[15px]"
              src="../../../assets/images/icons/right1.svg"
            />
          </p>
        </button>
        <!-- <input
          class="w-[100px] h-[40px] ml-auto bg-[#000167] rounded py-3 hover:bg-[#000267a9]"
          type="submit"
          value="Next ->"
        /> -->
      </form>
    </div>
  </div>
</template>

<script setup>
const handleSubmit = (e) => {
  e.preventDefault();
  const value = e.target.otp.value;
  if (value) {
    navigateTo("/api/v1/form");

    e.target.reset();
  } else {
    alert("Enter Otp");
  }
};
</script>

<style scoped></style>
