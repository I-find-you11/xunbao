<template>
  <div id="indexItem">
    <div class='period'>
      第<span>{{infor.period}}</span>期
    </div>
    <div class='goodsImg'>
      <img :src='infor.imgSrc' />
    </div>
    <div class='scheduleContainer'>
      <div class='schedule'></div>
      <div class='surface'>
        <span>参与人数</span>
        <span>{{infor.people}}</span>
      </div>
    </div>
    <div class='dateTime'>
      <div class='dateTimeIocnBg'>
        {{infor.dateTime}}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'indexItem',
  data() {
    return {

    }
  },
  props:['infor']
}
</script>

<style>
#indexItem {
  position: relative;
  width: 3.28rem;
  height: 4.17rem;
  background: rgba(255, 255, 255, .1);
  border-radius: .12rem;
  box-sizing: border-box;
  padding-top: .2rem;
}
.period {
  position: absolute;
  top: .07rem;
  left: .07rem;
  background: #7435a7;
  width: 1.06rem;
  height: .32rem;
  line-height: .32rem;
  border-radius: .05rem;
  font-size: .19rem;
  font-weight: bold;
}
.period span{
  color: #fff600;
}
.goodsImg {
  width: 3.1rem;
  margin: 0 auto;
}
.goodsImg img {
  width: 100%;
}
</style>
