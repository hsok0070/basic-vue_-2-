<template>
    <div>
        <h1>{{ title }}</h1>
        <p> {{ name }}</p>
        <button @click="updateName">Change Name</button>
    </div>
</template>

<script>
export default {
  data () {
    return {
      /* name: 'MinWoo' */ /* props에서 name을 사용하고 있기때문에 다른곳에서 사용 불가 */
    }
  },
  methods: {
    updateName () {
      this.name = 'MinWoo Updated'
    }
  },
  props: { /* 받은 데이터는 직접적으로 변경 불가능 하다 기존에 name을 변경하는 updateName() 메소드 동작은 하나 console창에 warn메시지가 나타난다. */
    title: {
      type: String,
      required: false,
      default: 'default title'
    },
    name: {
      type: String,
      required: false,
      default: 'default name'
    }
  }
}
</script>

<style  scoped>

</style>
