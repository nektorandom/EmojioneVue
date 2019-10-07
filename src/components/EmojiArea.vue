<template>
    <div class="rn-textare__wrapper">
        <textarea></textarea>

        <div class="rn-textare-inner__wrapper">
            <div class="rn-textare-editor" contenteditable="true" placeholder tabindex="0" dir="ltr" spellcheck="false" autocomlpete="false">
                Default test
            </div>

            <div class="emojiarea-btn__wrapper" title="Use Tab">
                <div class="emojiarea-btn open">
                    <i class="far fa-grin"></i>
                </div>
                <div class="emojiarea-btn--close"></div>
            </div>

            <div class="emojiarea-picker__wrapper">
                
            </div>
        </div>
    </div>
</template>

<style lang="scss">
  @import '@/assets/scss/templates/emojiarea.scss';
</style>