<template>
  <a
    :href="href"
    :target="target"
    class="inline-block rounded shadow-sm border border-green-800 text-green-900 hover:text-white hover:bg-green-800 py-3 px-4"
  >
    <slot></slot>
  </a>
</template>

<script lang="ts">
import Vue from 'vue'
import Component from 'nuxt-class-component'
import { Prop } from 'nuxt-property-decorator'

@Component
export default class ButtonPrimary extends Vue {
  @Prop()
  public readonly href: string | undefined

  @Prop({ default: '_blank' })
  public readonly target!: string
}
</script>

<style scoped></style>
