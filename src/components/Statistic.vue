<template>
  <div class="text-center">
    <h1 class="display-4">{{ statisticMainText }}</h1>
    <p class="lead" v-if="statisticSubText">{{ statisticSubText }}</p>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Card extends Vue {
  @Prop() private statisticMainText!: string;
  @Prop() private statisticSubText!: string;
}
</script>
