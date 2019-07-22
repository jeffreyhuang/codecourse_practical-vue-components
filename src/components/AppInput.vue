<template>
  <div>
    <input
      :type="inputType"
      :name="name"
      :id="name"
      class="form-control"
    >
    <a
      href="#"
      v-if="type === 'password'"
      @click.prevent="toggleVisibility"
    >Reveal password</a>
  </div>
</template>

<script>
export default {
  data () {
    return {
      inputType: this.type
    }
  },

  props: {
    name: {
      type: String,
      required: true
    },
    type: {
      type: String,
      required: false
    }
  },

  methods: {
    toggleVisibility () {
      this.inputType = this.inputType === 'password' ? 'text': 'password'
    }
  }
}
</script>
