<script setup lang="ts">

const { t } = useI18n()

</script>
<template>
  <nav class="flex-row m-5">
    <router-link class="icon-btn mx-2" to="/holidayCalculator" :title="t('menu.home')">
      <span>
        <carbon-calculator />
        {{ t('menu.holiday-calculator.title') }}
      </span>
    </router-link>
    <router-link class="icon-btn mx-2" to="/holidayCalculator" :title="t('menu.home')">
      <span>
        <carbon-calculator />
        {{ t('menu.holiday-calculator.title') }}2
      </span>
    </router-link>
    <router-link class="icon-btn mx-2" to="/holidayCalculator" :title="t('menu.home')">
      <span>
        <carbon-calculator />
        {{ t('menu.holiday-calculator.title') }}3
      </span>
    </router-link>
  </nav>
</template>
