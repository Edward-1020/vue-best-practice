<template lang="html">
    <div>
      <Heador/>
      <HomeSlider/>
      <Novice/>
    </div>
</template>

<script>
import Heador from '../public/header'
import HomeSlider from './home-slide'
import Novice from './novice'

export default {
  components: {
    Heador,
    HomeSlider,
    Novice
  }
}
</script>

<style lang="scss" module>

</style>
