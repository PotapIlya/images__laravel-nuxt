<template>
  <div class="input-wrapper">
    <span>{{ label }}</span>
    <label for="">
      <input
        :placeholder="placeholder"
        :value="defaultValue"
        type="text"
      >
    </label>
  </div>
</template>

<script>
  export default {
    props: {
      label: {
        type: String,
        required: false,
      },
      placeholder: {
        type: String,
        required: false,
      },
      defaultValue: {
        type: String,
        required: false,
        default: '',
      },
    }
  }
</script>
<style>
  .input-wrapper{
    display: flex;
    flex-direction: column;
  }
</style>
