<template>
  <div id='app'>
    <h1>This is Home page</h1>
    <MinWoo title='home title' name="MinWoo"></MinWoo>
  </div>
</template>

<script>
import MinWoo from '@/components/MinWoo.vue' /* @는 src위치를 가르킨다. */

export default {
  components: {
    MinWoo
  },
  data () {
    return {
      name: 'Min Woo'

    }
  }
}

</script>

<style scoped>
  h1 {
    color : red;
  }
</style>
