<template>
      <HeaderInner />
</template>

<script>
  import { defineComponent } from 'vue';
  import HeaderInner from './HeaderInner.vue';

  export default defineComponent({
    name: 'Header',
    components: {
      HeaderInner
    }
  })
</script>

