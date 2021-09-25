<script setup lang="ts">
import { useI18n } from 'vue-i18n'
const firstName = 'David'

const { t } = useI18n()
</script>

<template>
  <Tester last-name="Turgeon"></Tester>
  <h3>hello there, {{ firstName }}</h3>
  <h5>{{ t('intro.desc') }}</h5>
</template>
