<template>
  <div id="app">
    <Header />
    <Main :dischi ="dischi"/>
  </div>
</template>

<script>
import axios from 'axios'
import Header from './components/Header.vue'
import Main from './components/Main.vue'


export default {
  name: 'App',
  components: {
    Header,
    Main,
  },
  data () {
    return {
      dischi: []
    }
  },
  created() {
    axios.get('https://flynn.boolean.careers/exercises/api/array/music').then((result) => {
      this.dischi = result.data
    })
  }
}
</script>

<style lang="scss">

</style>
