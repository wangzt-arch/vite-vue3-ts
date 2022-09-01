<script setup lang="ts">
import { onMounted } from "vue";

interface Props {
  msg: string;
}

const props = defineProps<Props>();
console.log(props);

const message = "";
const msgClick = () => {
  console.log(message);
};
onMounted(() => {
  console.log("初始化");
});
</script>

<template>
  <h1 class="green" @click="msgClick">{{ msg }}</h1>
  {{ message }}
</template>

<style scoped></style>
