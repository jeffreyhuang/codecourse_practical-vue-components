<template>
  <div>
    {{ form }}

    <AppInput name="password" v-model="form.email"/>
  </div>
</template>

<script>
import AppInput from '@/components/AppInput'

export default {
  name: 'home',
  components: {
    AppInput
  },
  data () {
    return {
      form: {
        email: 'jeffrey@kingdomfullstack.com'
      }
    }
  }
}
</script>
