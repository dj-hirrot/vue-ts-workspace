<template>
  <button @click="onClick">MyButton</button>
</template>

<script lang="ts">
  import { Component, Prop, Vue } from "vue-property-decorator";

  @Component
  export default class MyButton extends Vue {
    @Prop()
    public greet?: string;

    public onClick() {
      alert(this.greet);
      this.greet = "$B$3$s$K$A$O(B";
    }
  }
</script>
