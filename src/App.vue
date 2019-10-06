<template>
  <div id="app">
      <emoji-area></emoji-area>
  </div>
</template>

<script>
import EmojiArea from './components/EmojiArea'

export default {
  name: 'app',
  components: {
    EmojiArea
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
