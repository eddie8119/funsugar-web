<template>

  <div class="modal fixed bg-white p-4 rounded-2xl z-10">
    <div class="flex flex-col w-full items-center">
      <label for="user_email" class="text-stone-500 text-left">E-mail</label>
      <input type="email" name="user_email" id="user_email" class="bg-stone-200 py-2 px-4 w-full mb-6 xl:w-[80%]">
      <label for="user_message" class="text-stone-500 text-left">訊息 Message</label>
      <textarea name="user_message" id="user_message" cols="30" rows="10"
        class="bg-stone-200 py-2 px-4 w-full mb-6 xl:w-[80%]"></textarea>
      <button class="btn w-full md:w-[80%]">送出</button>
    </div>
  </div>

</template>

<script>
export default {
  name: "CommissionForm",
  data() {
    return {
    };
  },
};
</script>
  
<style scoped>
.modal {
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100%;
  max-width: 40%;
}
</style>
  