<template>
  <button
    @click="$emit('event')"
    class="btn btn-info"
    :disabled="disabled"
  >
    {{ label }}
  </button>
</template>

<script>
  export default {
    props: {
      label: {
        type: String,
        required: true,
      },
      disabled: {
        type: Boolean,
        required: false,
      }
    }
  }
</script>
