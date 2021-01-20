<template>
  <Swiper class="swi">
    <SwiperItem v-for="(item,index) in topImages" :key="index">
      <img :src="item" alt />
    </SwiperItem>
  </Swiper>
</template>

<script>
import { Swiper, SwiperItem } from "components/common/swiper";

export default {
  name: "DetailSwiper",
  components: {
    Swiper,
    SwiperItem,
  },
  props: {
    topImages: {
      type: Array,
      default() {
        return [];
      },
    },
  },
};
</script>

<style scoped>
.swi {
  height: 300px;
  overflow: hidden;
}
</style>