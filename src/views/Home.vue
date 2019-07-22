<template>
  <div>
    <AppInput name="password" placeholder="e.g. jeffrey@kingdomfullstack.com"/>
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
