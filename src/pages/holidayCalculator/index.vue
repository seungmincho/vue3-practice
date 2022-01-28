<script setup lang="ts">
const joinDate = ref('')
const onClickHolidaycalculation = () => {
  console.log(joinDate)
}
const { t } = useI18n()
</script>

<template>
  <div>
    <p>
      {{ t('menu.holiday-calculator.title') }}
    </p>
    <div>
      <label>{{ t('menu.holiday-calculator.joinDate') }}:</label>
      <input
        id="input-joinDate"
        v-model="joinDate"
        type="date"
        m="x-2 y-2"
        p="y-0"
        text="center"
        bg="transparent"
        outline="solid-gray-500"
        @keydown.enter="onClickHolidaycalculation"
      >
    </div>
    <div>
      <button
        class="m-3 text-sm btn"
        :disabled="!joinDate"
        @click="onClickHolidaycalculation"
      >
        {{ t('button.calculation') }}
      </button>
    </div>
    <span>
      {{ joinDate }}
    </span>
  </div>
</template>
