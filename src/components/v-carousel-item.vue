<template>
    <div class="v-carousel-item">
        <img :src='require("../assets/images" + item_data.image)'>
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