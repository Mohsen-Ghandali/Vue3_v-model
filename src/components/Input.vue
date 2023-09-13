<template>
  <div>
    <input
      type="text"
      :value="modelValue"
      @input="$emit('update:modelValue, $event.target.value')"
    />
  </div>
</template>

<script lang="ts">
export default {
  name: 'Input',
  props: {
    modelValue: String,
  },
};
</script>

<style lang="scss" scoped></style>
