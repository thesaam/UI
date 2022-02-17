<script>
  import icon from "./icons/Icon.png"

  export default {
    name: 'Button',
    data: function () {
      return{
        image:icon
      }
    },
  }
</script>

<template>
  <div class="px-3">
    <button class="btn d-flex"><img class="px-1 pt-1" :src="image">Upgrade now</button>
  </div>
</template>

<style>
  .btn {
    border: 2px solid #D0D5DD;
    border-radius: 8px;
    color: #344054;
    font-weight: 500;
    line-height: 24px;
  }
</style>

