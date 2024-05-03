<template>
  <nut-input v-model="val" placeholder="添加记事..." clearable>
    <template #right>
      <Check @click="console.log('Check')" style="margin-right: 1rex" />
      <Photograph />
    </template>
  </nut-input>
</template>
<script setup>
import { ref } from "vue";
import { Checkbox, CheckboxGroup } from "@nutui/nutui-taro";
import { Photograph, Check } from "@nutui/icons-vue-taro";
const val = ref("");
const run = ref(false);
</script>
