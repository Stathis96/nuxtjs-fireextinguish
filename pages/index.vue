<template>
  <div>
    <Hero />
    <LargeCardDisplay
      v-for="cardInfo in largeCardInfo"
      :key="cardInfo.id"
      :cardsection="cardInfo"
    />
    <SmallCardDisplay
      v-for="cardInfo in smallCardSections"
      :key="cardInfo.id"
      :cardsection="cardInfo"
    />
  </div>
</template>

<script>
import { largeCardSections, smallCardSections } from '@/assets/data.js'
export default {
  data () {
    return {
      largeCardInfo: largeCardSections,
      smallCardSections
    }
  }
}
</script>

<style>
</style>
