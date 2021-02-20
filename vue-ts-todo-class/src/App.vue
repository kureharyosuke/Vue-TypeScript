<template>
  <div>
    <h1>Vue Typescript Class</h1>
    <todo-input :item="todoText"></todo-input>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import TodoInput from "../../vue-ts-todo/src/components/TodoInput.vue";

@Component({
  components: {
    TodoInput
  }
})
export default class extends Vue {
  data() {
    return {
      todoText: ""
    };
  }
}
</script>

<style scoped></style>
