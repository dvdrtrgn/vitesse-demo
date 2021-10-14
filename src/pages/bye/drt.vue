<script setup lang="ts">
import { useI18n } from 'vue-i18n'
import aMarkdownFile from './aMarkdownFile.md'
const firstName = 'David'

const { t } = useI18n()
</script>

<template>
  <aMarkdownFile></aMarkdownFile>

  <Tester class="bg-lime-400 rounded-1" last-name="Turgeon"></Tester>

  <h3 class="text-4xl text-red-500">
    Goodbye, {{ firstName }}
  </h3>

  <h5>{{ t('intro.desc') }}</h5>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
