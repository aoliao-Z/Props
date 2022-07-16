<script lang="ts" setup>
import Children from "./Children.vue";
import { ref } from "vue";
const name = ref("a");
setTimeout(() => {
  name.value = "b";
}, 1000);
</script>

<template>
  <div>
    <Children :name="name" />
  </div>
</template>