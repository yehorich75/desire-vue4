<template>
    <div class="top__slider">
        <div class="v-carousel">
            <vCarouselItem
                v-for="item in carousel_data"
                :key="item.id"
                :item_data="item"
                :imageSlide="false"
                :width="sliderWidth"
                />
        </div>
    </div>
</template>

<script>

    import vCarouselItem from './v-carousel-item.vue';

    export default {
        name: "v-carousel",
        components: {
            vCarouselItem
        },
        props: {
            carousel_data: {
                type: Array,
                default: () => []
            },
            interval: {
                type: Number,
                default: 0
            },
            slideWidth: {
                type: Number,
                default: 300
            }
        },
        data() {
            return {}
        },
        computed: {}
    }
</script>

<style scoped>

</style>