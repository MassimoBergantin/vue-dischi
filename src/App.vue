<template>
  <div id="app">
    <Header />
    <Main :poster ="poster"/>
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
      poster: []
    }
  },
  created() {
    axios.get('https://flynn.boolean.careers/exercises/api/array/music').then((result) => {
      this.poster = result.data.result
    })
  }
}
</script>

<style lang="scss">
 @import "./style/app.scss"
</style>
