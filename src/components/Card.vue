<template>
  <div class="card border-0 shadow-sm p-3">
    <h5 class="card-title" v-if="title">{{ title }}</h5>
    <h6 class="card-subtitle mb-2 text-muted" v-if="subtitle">{{ subtitle }}</h6>
    <slot></slot>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Card extends Vue {
  @Prop() private title!: string;
  @Prop() private subtitle!: string;
  @Prop() private text!: string;
}
</script>
