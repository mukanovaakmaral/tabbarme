<template>

  <AlserTabbar :tabs="tab" />

</template>

<script setup lang="ts">

import AlserTabbar from "@/components/AlserTabbar.vue";
import {ref, Ref} from "vue";

const tab: Ref<any> = ref([
  {value:'text'},
  {value:'istext'},
  {value:'istext'},
  {value:'istext'}
])

</script>

<style scoped>

</style>