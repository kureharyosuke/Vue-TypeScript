<template>
  <div>
    <label for="todo-input"></label>
    <input id="todo-input" type="text" :value="todoText" />
    <button @click="onClickInput" type="button"></button>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class extends Vue {
  @Prop({ default: "" })
  item!: string;

  private onClinkInput(): void {
    console.log("click input");
  }
}
</script>

<style scoped></style>
