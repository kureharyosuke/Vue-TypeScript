<template>
  <div>
    <label for="todo-input"></label>
    <input id="todo-input" type="text" />
    <button @click="onClickInput" type="button"></button>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class extends Vue {
  private onClinkInput(): void {
    console.log("click input");
  }
}
</script>

<style scoped></style>
