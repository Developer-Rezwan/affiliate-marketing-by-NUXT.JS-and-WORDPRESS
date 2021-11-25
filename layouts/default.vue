<template>
  <div>
    <TheHeader />
    <div class="bg-gray-100">
      <slot />
    </div>

    <TheFooter />
  </div>
</template>

<script lang="ts">
import TheHeader from "./../components/TheHeader.vue"
import TheFooter from "./../components/TheFooter.vue"
export default {
  components: { TheHeader, TheFooter },
}
</script>

<style>
</style>