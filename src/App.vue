<script>
import partHeader from './components/partHeader.vue';
import partMiddle from './components/partMiddle.vue';
import partFooter from './components/partFooter.vue'

export default {

  components: {
    partHeader,
    partMiddle,
    partFooter
  }

}
</script>

<template>
  <partHeader />
  <partMiddle />
  <partFooter />
</template>

<style lang="scss">
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
</style>
