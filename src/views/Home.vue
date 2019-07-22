<template>
  <div>
    <AppLabel forInput="email">
      Enter your email address
    </AppLabel>
    <AppInput name="email" placeholder="e.g. jeffrey@kingdomfullstack.com"/>
  </div>
</template>

<script>
import AppInput from '@/components/AppInput'
import AppLabel from '@/components/AppLabel'

export default {
  name: 'home',
  components: {
    AppInput,
    AppLabel
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
