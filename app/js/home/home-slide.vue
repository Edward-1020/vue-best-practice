<template>
  <article class="">
    <Slider :items="items" :cname="$style.slider"/>
    <section :class="$style.list">
      <div :class="$style.item" v-for="item in enters" :key="item.img">
        <router-link :to="{name: item.href}">
          <img :src="item.img" :alt="item.title">
          <h4>{{item.title}}</h4>
        </router-link>
      </div>
    </section>
  </article>
</template>

<script type="text/ecmascript-6">
import Slider from '../core/slider'

export default {
  data () {
    return {
      items: [{
        href: 'home',
        src: '//img12.360buyimg.com/jrpmobile/jfs/t14785/52/2084715101/47599/b4825059/5a672ea7N80b7d3df.jpg?width=750&height=320'
      }, {
        href: 'home',
        src: '//img12.360buyimg.com/jrpmobile/jfs/t18274/116/259410275/46959/87ec4b20/5a672ef0N6b18360d.jpg?width=750&height=320'
      }, {
        href: 'home',
        src: '//img12.360buyimg.com/jrpmobile/jfs/t18616/275/262454992/43455/e59743b5/5a672f31N03cf5491.jpg?width=750&height=320'
      }],
      enters: [{
        href: 'home',
        img: '//img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
        title: '优惠券'
      }, {
        href: 'home',
        img: '//img12.360buyimg.com/jrpmobile/jfs/t5590/252/875247023/17343/946aa72c/59224650N0f7ffc92.png?width=132&height=132',
        title: '领红包'
      }, {
        href: 'home',
        img: '//img12.360buyimg.com/jrpmobile/jfs/t4393/329/2180608902/13217/c88c0cec/58ec9dcdN1534e2d7.png?width=132&height=132',
        title: '抢钢镚'
      }, {
        href: 'home',
        img: '//img12.360buyimg.com/jrpmobile/jfs/t4618/115/2179710654/11347/bf520df/58ec9d84Nfd169001.png?width=132&height=132',
        title: '领京豆'
      }, {
        href: 'home',
        img: '//img12.360buyimg.com/jrpmobile/jfs/t5488/298/1036263348/12073/b4f4de97/590ac8e8Ne9def22e.png?width=135&height=135',
        title: '白条提额'
      }]
    }
  },
  components: {
    Slider
  }
}
</script>

<style lang="scss" rel="stylesheet/scss" module>
@import '../../css/element.scss';

.slider {
  margin-top: 120px;
  img {
    width: 100%;
  }
}

.list {
  @include list(row);
  background: #fff;
  padding-top: 40px;
  padding-bottom: 20px;
  justify-content: space-around;
  a {
    text-decoration: none;
  }
  .item {
    text-align: center;
    img {
      display: inline-block;
      width: 90px;
      height: 90px;
    }
    h4 {
      font-size: 26px;
      margin-top: 12px;
      color: #666;
    }
  }
}
</style>