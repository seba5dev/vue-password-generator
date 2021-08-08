<template>
<div id="app">
  <Password></Password>
</div>
<div id="app">
  <Password2></Password2>
</div>
</template>

<script>
import Password from './components/Password.vue'
import Password2 from './components/Password2.vue'

export default {
  name: 'App',
  components: {
    Password,
    Password2
  }
}
</script>
