<template>
  <a
    :href="href"
    :target="target"
    class="inline-block rounded shadow-sm border border-gray-800 text-gray-900 hover:text-white hover:bg-gray-800 py-3 px-4"
  >
    <slot></slot>
  </a>
</template>

<script lang="ts">
import Vue from 'vue'
import Component from 'nuxt-class-component'
import { Prop } from 'nuxt-property-decorator'

@Component
export default class ButtonSecondary extends Vue {
  @Prop()
  public readonly href: string | undefined

  @Prop({ default: '_blank' })
  public readonly target!: string
}
</script>

<style scoped>
.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
