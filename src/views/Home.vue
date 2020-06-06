<template>
  <div id='app'>
    <h1>This is Home page</h1>
    <!-- <MinWoo title='home title' name="MinWoo"></MinWoo> --> <!-- 부모 컴포넌트로 데이터 보내기 공부 하기 위해 주석 -->
    <form action="">
      <InputField @update-name='name = $event.target.value'></InputField>
      <!-- <InputField v-model="name"></InputField --> <!-- 위 $event를 간단히 사용하는방법 -->
      <br><br><button>Submit</button>
    </form>
    {{ name }}
  </div>
</template>

<script>
/* import MinWoo from '@/components/MinWoo.vue' */
import InputField from '@/components/InputField.vue'

export default {
  components: {
    InputField
  },
  data () {
    return {
      name: ''

    }
  }
  /* methods: {
    updateName (name) {
      this.name = name
    }
  } */
}

</script>

<style scoped>
  h1 {
    color : red;
  }
</style>
