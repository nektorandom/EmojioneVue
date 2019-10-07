<template>
  <div id="app" class="rn-main__wrapper">
    <h1>Example emoji textarea</h1>
    
    <div class="rn-padding-sm rn-with-1-2">
      <emoji-area></emoji-area>
    </div>
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

<style lang="scss">
  @import url('https://fonts.googleapis.com/css?family=Unica+One'); // TODO::

  @import '@/assets/scss/parts/_common.scss';
  @import '@/assets/scss/parts/_btn.scss';
  @import '@/assets/scss/parts/_textarea.scss';
</style>
