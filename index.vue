<template>
  <button>
    {{ modelValue }}
  </button>
</template>

<script>
const getModel = (prop = 'modelValue', event = `update:${prop}`) => ({
  prop,
  event,
});

export default {
  model: getModel(),

  props: {
    modelValue: {
      type: String,
      default: Button,
    },
  },
};
</script>
