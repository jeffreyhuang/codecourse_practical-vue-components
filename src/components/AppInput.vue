<template>
  <div>
    <input
      :type="inputType"
      :name="name"
      :id="name"
      class="form-control"
      :value="value"
      @input="$emit('input', $event.target.value)"
    >
    <a
      href="#"
      v-if="type === 'password'"
      @click.prevent="passwordRevealed = !passwordRevealed"
    >
      {{ passwordRevealed ? 'Hide' : 'Reveal' }} password
    </a>
  </div>
</template>

<script>
export default {
  data () {
    return {
      passwordRevealed: false
    }
  },

  props: {
    value: {
      type: String,
      required: false,
      default: ''
    },
    name: {
      type: String,
      required: true
    },
    type: {
      type: String,
      required: false
    }
  },

  computed: {
    inputType () {
      return this.passwordRevealed ? 'text' : this.type
    }
  }
}
</script>
