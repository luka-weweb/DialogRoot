<script>
export default {
  props: {
    content: { type: Object, required: true },
    wwFrontState: { type: Object, required: true },
    wwEditorState: { type: Object, required: true },
  },
  emits: ["trigger-event"],
  data() {
    return {
      tabTriggers: [],
      internalActiveTab: this.content.controlled
        ? this.content.default
        : this.content.modelValue,
    };
  },
};
</script>

<template>
  <wwElement />
</template>
