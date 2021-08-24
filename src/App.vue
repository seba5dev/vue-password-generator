<template>
<div id="app">
  <Password></Password>
</div>

<div id="app">
  <Password2></Password2>
</div>

<div id="app">
    <Password3></Password3>
</div>
</template>

<script>
import generatePassword from "custom-password-generator";

import Password from './components/Password.vue'
import Password2 from './components/Password2.vue'
import Password3 from './components/Password3.vue'

export default {
  name: 'App',
  components: {
    Password,
    Password2,
    Password3
  }
}
</script>
