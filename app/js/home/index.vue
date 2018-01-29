<template lang="html">
    <div>
      <Heador/>
      <HomeSlider/>
      <Novice/>
      <Borrow/>
      <Money/>
      <Product/>
      <Life/>
      <Footor/>
      <Navbar/>
    </div>
</template>

<script>
import Heador from '../public/header'
import HomeSlider from './home-slide'
import Novice from './novice'
import Borrow from './borrow'
import Money from './money'
import Product from './product'
import Life from './life'
import Footor from '../public/Footer'
import Navbar from '../public/navbar'

export default {
  components: {
    Heador,
    HomeSlider,
    Novice,
    Borrow,
    Money,
    Product,
    Life,
    Footor,
    Navbar
  }
}
</script>

<style lang="scss" module>

</style>
