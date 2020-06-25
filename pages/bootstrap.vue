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
        <a
          class="btn btn-lg btn-outline-primary"
          href="https://nuxtjs.org/"
          target="_blank"
          role="button"
          >Documentation</a
        >
        <a
          class="btn btn-lg btn-outline-secondary"
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          role="button"
          >GitHub</a
        >
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'
// eslint-disable-next-line @typescript-eslint/no-unused-vars,no-unused-vars
import bootstrap from 'bootstrap'
import Logo from '@/components/Logo.vue'
import ButtonPrimary from '~/components/ButtonPrimary.vue'
import ButtonSecondary from '~/components/ButtonSecondary.vue'

@Component({ components: { ButtonPrimary, ButtonSecondary, Logo } })
export default class Bootstrap extends Vue {}
</script>

<style lang="scss">
@import '~bootstrap/scss/bootstrap';
</style>
