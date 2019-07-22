<template>
  <input
    type="text"
    :name="name"
    :id="name"
    class="form-control"
  >
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true
    }
  }
}
</script>
