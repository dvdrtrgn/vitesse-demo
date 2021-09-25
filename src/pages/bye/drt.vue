<script setup lang="ts">
import { useI18n } from 'vue-i18n'
import Zinfo from '~/pages/bye/Zinfo.md'
const firstName = 'David'

const { t } = useI18n()
</script>

<template>
  <Zinfo></Zinfo>
  <Tester class="bg-lime-400 rounded-1" last-name="Turgeon"></Tester>
  <h3 class="text-4xl text-red-500">
    hello there, {{ firstName }}
  </h3>
  <h5>{{ t('intro.desc') }}</h5>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
