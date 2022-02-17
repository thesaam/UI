<script>
  import upload from "./icons/upload.png"
  import plus from "./icons/plus.png"

  export default {
    name: "Header",

    data: function () {
      return {
        upload: upload,
        plus: plus
      }
    }
  }
</script>

<template>
  <header class="d-flex px-5 py-5 justify-content-between">
    <div class="left">
      <h2>Welcome back, Olivia</h2>
      <p class="header-text">Track, manage and forecast your customers and orders.</p>
    </div>
    <div>
      <button class="btn px-3 mx-3 text-center "><img :src="upload" class="px-2" >Import </button>
      <button class="btn btn-1 px-3"><img :src="plus" class="px-2" >Add</button>
    </div>
  </header>
</template>

<style scoped>
 .btn-1 {
   background: #7F56D9;
   color: #fff;
 }

 .header-text {
   color: #667085;
 }
</style>