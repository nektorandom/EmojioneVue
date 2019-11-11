<template>
    <div class="rn-textare__wrapper">
        <div class="rn-textare-inner__wrapper emojiarea__wrapper" :class="{'active': this.setIsOpen === true}">
            <div class="rn-textare-editor" contenteditable="true" placeholder tabindex="0" dir="ltr" spellcheck="false" autocomlpete="false">
                Default test
            </div>

            <div class="emojiarea-btn__wrapper" title="Use Tab">
                <div class="emojiarea-btn open" @click="openModal">
                    <i class="far fa-grin"></i>
                </div>
                <div class="emojiarea-btn--close"></div>
            </div>

            <div class="emojiarea-picker__wrapper emojionearea-picker-position-top">
                <div class="emojiarea-picker">
                    <div class="emojiarea-filters">
                        <i class="emojiarea-filter emojiarea-filter-recent" data-filter="recent" title="Recent" style="">
                            <img class="emojioneemoji" src="https://cdn.jsdelivr.net/emojione/assets/3.1/png/32/1f552.png">
                        </i>
                        <i class="emojiarea-filter emojiarea-filter-smileys_people active" data-filter="smileys_people" title="Smileys &amp; People">
                            <img class="emojioneemoji" src="https://cdn.jsdelivr.net/emojione/assets/3.1/png/32/1f60b.png">
                        </i>
                        <i class="emojiarea-filter emojiarea-filter-animals_nature" data-filter="animals_nature" title="Animals &amp; Nature">
                            <img class="emojioneemoji" src="https://cdn.jsdelivr.net/emojione/assets/3.1/png/32/1f439.png">
                        </i>
                        <i class="emojiarea-filter emojiarea-filter-food_drink" data-filter="food_drink" title="Food &amp; Drink">
                            <img class="emojioneemoji" src="https://cdn.jsdelivr.net/emojione/assets/3.1/png/32/1f355.png">
                        </i>
                        <i class="emojiarea-filter emojiarea-filter-activity" data-filter="activity" title="Activity">
                            <img class="emojioneemoji" src="https://cdn.jsdelivr.net/emojione/assets/3.1/png/32/1f3c0.png">
                        </i>
                        <i class="emojiarea-filter emojiarea-filter-travel_places" data-filter="travel_places" title="Travel &amp; Places">
                            <img class="emojioneemoji" src="https://cdn.jsdelivr.net/emojione/assets/3.1/png/32/1f680.png">
                        </i>
                        <i class="emojiarea-filter emojiarea-filter-objects" data-filter="objects" title="Objects">
                            <img class="emojioneemoji" src="https://cdn.jsdelivr.net/emojione/assets/3.1/png/32/1f4a1.png">
                        </i>
                        <i class="emojiarea-filter emojiarea-filter-symbols" data-filter="symbols" title="Symbols">
                            <img class="emojioneemoji" src="https://cdn.jsdelivr.net/emojione/assets/3.1/png/32/1f497.png">
                        </i>
                        <i class="emojiarea-filter emojiarea-filter-flags" data-filter="flags" title="Flags">
                            <img class="emojioneemoji" src="https://cdn.jsdelivr.net/emojione/assets/3.1/png/32/1f1ec-1f1e7.png">
                        </i>
                    </div>

                    <div class="emojiarea-search-panel emojiarea-with-search">
                        <div class="emojiarea-search">
                            <input placeholder="SEARCH" type="text" class="search">
                        </div>

                        <div class="emojiarea-tones emojiarea-tones-bullet">
                            <i class="btn-tone btn-tone-0 active" data-skin="0" role="button"></i>
                            <i class="btn-tone btn-tone-1" data-skin="1" role="button"></i>
                            <i class="btn-tone btn-tone-2" data-skin="2" role="button"></i>
                            <i class="btn-tone btn-tone-3" data-skin="3" role="button"></i>
                            <i class="btn-tone btn-tone-4" data-skin="4" role="button"></i>
                            <i class="btn-tone btn-tone-5" data-skin="5" role="button"></i>
                        </div>
                    </div>

                    <div class="emojiarea-scroll-area">
                        <div class="emojiarea-emojis-list">

                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import mixin from './mixin';

    export default {
        mixins: [
            mixin
        ]
    }
</script>

<style lang="scss">
  @import '@/assets/scss/templates/emojiarea.scss';
</style>