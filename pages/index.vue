<template>
  <div class="flex min-h-screen justify-center items-center text-center">
    <div>
      <logo />
      <h1 class="text-6xl text-blue-900 text-capitalize">
        Luminis Frontend Meeting
      </h1>
      <h2 class="text-4xl text-blue-800 mb-3">
        My swell Nuxt.js project
      </h2>
      <div class="mt-3">
        <button-primary href="https://nuxtjs.org/">
          Documentation
        </button-primary>

        <button-secondary href="https://github.com/nuxt/nuxt.js">
          GitHub
        </button-secondary>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
import Logo from '@/components/Logo.vue'
import ButtonPrimary from '~/components/ButtonPrimary.vue'
import ButtonSecondary from '~/components/ButtonSecondary.vue'

@Component({ components: { ButtonPrimary, ButtonSecondary, Logo } })
export default class Index extends Vue {}
</script>

<style lang="scss"></style>
