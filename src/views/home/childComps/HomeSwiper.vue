<template>
  <swiper>
      <swiper-item v-for="(item,key) in banners" :key="key">
        <a :href="item.link">
          <img :src="item.image" alt="">
        </a>
      </swiper-item>
    </swiper>
</template>

<script type="text/javascript">
import {Swiper,SwiperItem} from 'components/common/swiper'
export default {
  name: "HomeSwiper",
  data() {
    return {

    }
  },
  props:{
      banners:{
          type:Array,
          default(){
              return[]
          }
      }
  },
  components: {
      Swiper,
      SwiperItem
  }
}
</script>

<style scoped>
</style>
