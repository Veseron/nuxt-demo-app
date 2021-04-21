<template>
  <div class="container">
    <Hero/>
    <LargeCardDisplay 
      v-for="largeCardInfo in largeCardInfo"
      :key="largeCardInfo.id"
      :cardsSection="largeCardInfo"
    />
    <SmallCardDisplay
      v-for="smallCardInfo in smallCardInfo"
      :key="smallCardInfo.id"
      :cardsSection="smallCardInfo"
    />
  </div>
</template>

<script>
import {largeCardSections, smallCardSections} from '@/assets/data.js'
export default {
  data() {
    return {
      largeCardInfo: largeCardSections,
      smallCardInfo: smallCardSections
    }
  }
}
</script>

<style>

</style>
