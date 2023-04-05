<template>
  <div class="w-full h-screen flex justify-center items-center">
    <div
      class="bg-[#00763A] w-[400px] shadow-black shadow-md p-5 grid grid-cols-1 gap-7 font-sans text-white rounded"
    >
      <h2 class="text-2xl font-bold text-center mt-5">User Info</h2>
      <form @submit="handleSubmit" class="w-full flex flex-col gap-6">
        <div>
          <!-- <label class="text-lg font-semibold" for="name">Name :</label> -->
          <input
            required
            placeholder=" Name"
            class="h-[40px] w-full rounded text-black overflow-x-scroll font-sans font-semibold"
            type="text"
            name="name"
            id=""
          />
        </div>
        <div>
          <!-- <label class="text-lg font-semibold" for="email">Email :</label> -->
          <input
            placeholder=" Email"
            required
            class="w-full h-[40px] rounded text-black overflow-x-scroll font-sans font-semibold"
            type="email"
            name="email"
            id=""
          />
        </div>
        <button
          class="w-1/2 mx-auto flex items-center justify-center h-[40px] content-center ml-auto bg-[#000167] rounded py-3 hover:bg-[#000267a9]"
          type="submit"
        >
          <p>Submit</p>
        </button>
      </form>
    </div>
  </div>
</template>

<script setup>
// definePageMeta({ layout: "admin" });
const handleSubmit = (e) => {
  e.preventDefault();
};
</script>

<style lang="scss" scoped></style>
