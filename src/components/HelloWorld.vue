<script setup lang="ts">
import { onMounted } from 'vue';

interface Props {
  msg: string
}

const props = defineProps<Props>()
const message = props.msg
const msgClick = () => {
  console.log(message);
}
onMounted(() => {
  console.log("初始化");
})

</script>

<template>
  <h1 class="green">{{ msg }}</h1>
  {{ message }}
</template>

<style scoped>
</style>
