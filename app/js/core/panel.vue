<template>
  <section :class="[panelClass, cname]">
    <h4>-{{ title }}-</h4>
    <slot/>
  </section>
</template>

<script type="text/ecmascript-6">
  export default {
    props: {
      cname: {
        type: String,
        default: ''
      },
      title: {
        type: String,
        default: ''
      }
    },
    data () {
      return {
        panelClass: 'panel'
      }
    }
  }
</script>

<style scoped lang="scss" rel="stylesheet/scss">
  @import '../../css/element.scss';

  .panel {
    @include panel;
  }
</style>