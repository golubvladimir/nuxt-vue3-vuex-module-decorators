<template>
  <div class="container">
  </div>
</template>

<script lang="ts">
import { defineComponent, useStore, computed } from "@nuxtjs/composition-api";

export default defineComponent({
  setup() {
    const store = useStore();

    const example = computed(() => store.state.example.count);

    console.log({book});
  }
})
</script>

<style>

</style>
