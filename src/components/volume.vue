<template>
  <div id="volume">
    <indexTitle name='卷' />
    <indexList :itemlist='list' />
  </div>
</template>

<script>
import indexTitle from '@/components/indexTitle'
import indexList from '@/components/indexList'

import goodsImg from '@/assets/img/prizeimage_small_1.png'
export default {
  name: 'volume',
  data() {
    return {
      list:[{
        period:'3',
        imgSrc:goodsImg,
        content:'看漫画专用',
        money:'126.000',
        people:'208',
        schedule:'95.67',
        dateTime:'00:05:55'
      }]
    }
  },
  components: {
    indexTitle,
    indexList
  }
}
</script>

<style>
.title {
    width: 2.41rem;
    height: .7rem;
    background: #472093;
    border: .05rem solid #864cba;
}
</style>
