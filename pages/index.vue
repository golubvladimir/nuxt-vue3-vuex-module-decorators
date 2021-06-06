<template>
  <div class="container">
  </div>
</template>

<script lang="ts">
import Example from "~/store/example";

export interface State {
  example: Example
}

import { defineComponent, useStore, computed } from "@nuxtjs/composition-api";

export default defineComponent({
  setup() {
    const store = useStore<State>();

    console.log(store.state.example.wheels);
  }
})
</script>

<style>

</style>
