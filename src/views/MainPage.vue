<template>
  <div>
    <HeaderBlock />
    <MainBlock />
  </div>
</template>

<script>
// @ is an alias to /src
// import Card from '@/components/elements/Card'
import HeaderBlock from '@/components/blocks/HeaderBlock.vue'
import MainBlock from '@/components/blocks/MainBlock.vue'

export default {
  name: 'MainPage',
  components: {
    HeaderBlock, MainBlock
  },
  props: {}
}
</script>
<style lang="scss" scoped></style>
