<template lang="html">
  <div>
    <span>{{text}}</span>
    <q-btn icon="create" @click="sayHi">Click to speak</q-btn>
  </div>
</template>

<script>
import { QBtn } from 'quasar'

export default {
  data() {
    text: ''
  },
  components: {
    QBtn
  },
  methods: {
    sayHi() {
      console.log("You clicked me.")
    	responsiveVoice.speak('hi there!')
      this.text = 'Hi there!'
    }
  }
}
</script>

<style lang="css">
</style>
