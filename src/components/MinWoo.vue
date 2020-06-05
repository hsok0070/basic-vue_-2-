<template>
    <div>
        <p> {{ name }}</p>
        <button @click="updateName">Change Name</button>
    </div>
</template>

<script>
export default {
  data () {
    return {
      name: 'MinWoo'
    }
  },
  methods: {
    updateName () {
      this.name = 'MinWoo Updated'
    }
  }
}
</script>

<style  scoped>

</style>
