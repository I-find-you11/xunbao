<template>
  <div id="indexList">
    <indexItem v-for='item in itemlist' :key='item.money' :infor='item' />
  </div>
</template>

<script>
import indexItem from '@/components/indexItem'
export default {
  name: 'indexList',
  data() {
    return {
      
    }
  },
  props:{
    itemlist: {
      Type: Array,
      default: () => []
    }
  },
  components: {
    indexItem
  }
}
</script>

<style>
</style>
