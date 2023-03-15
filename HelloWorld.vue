<template>
  <div class="tab-naming">
    <div v-for="tab in tabs"
         class="tab"
         :style="{ width: tabWidth + '%' }"
         :class="{ activeTab: activeTab === index }"
         @click="activeTab = index">
      {{ tab.value }}
    </div>

    <div class="line-wrapper">
      <div
          :style=" { width: avtiveTab + '%', left:(activeTab * this.avtiveTab) + '%'}"
          class="line"
      >
      </div>
    </div>

  </div>
</template>

<script setup lang="ts">


const props = defineProps({
  tabs: {
    type: Array,
    required: true,
  }
})


</script>

<style scoped>
.tab-naming {
  display: flex;
  width: 100%;
  align-items: center;
}


</style>