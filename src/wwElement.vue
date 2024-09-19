<template>
  <wwElement v-bind="content.contentElement" />
</template>

<script>
export default {
  props: {
    content: { type: Object, required: true },
    wwFrontState: { type: Object, required: true },
    wwEditorState: { type: Object, required: true },
  },
};
</script>
