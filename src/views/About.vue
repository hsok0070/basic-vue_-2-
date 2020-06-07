<template>
  <div class="about">
    <h1>This is an about page</h1>
    <MinWoo>
      <template #header="props"> <!-- v-slot은 #으로 줄여서 사용가능 -->
        <p>header11 {{ props.test}}</p>
      </template>
      <template #default>
        <div>
          hello11
        </div>
      </template>
    </MinWoo>
  </div>
</template>

<script>
import MinWoo from '@/components/MinWoo'

export default {
  components: {
    MinWoo
  }
}
</script>
