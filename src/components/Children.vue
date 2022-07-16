<script lang="ts" setup>
import { defineProps, computed } from "vue";
type ChildrenProps = {
  name: string;
};
const props = defineProps<ChildrenProps>();
const a = computed(() => {
  return props.name + "!";
});
</script>

<template>
  <div>
    {{ a }}
  </div>
</template>