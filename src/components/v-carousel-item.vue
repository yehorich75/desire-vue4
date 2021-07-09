<template>
    <div class="v-carousel-item">
        <img :src='require("../assets/images" + item_data.image) :alt="item_data.alt">
    </div>
</template>


<script lang=" js">
    export default {
        name: 'VCarouselItem',
        props: {
            item_data: {
                type: Object,
                default: () => {}
            }
        },
        data() {
            return {}
        },
        computed: {}
    }
</script>