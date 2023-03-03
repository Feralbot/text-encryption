<template>
  <v-sheet
    :min-height="450"
    class="border rounded-lg fill-height bg-grey-darken-1"
  >
    <p class="text-h4">Text is:</p>
    <p class="mx-2">
      {{ InputedText || "Load or enter text in field bellow" }}
    </p>
  </v-sheet>
</template>

<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  InputedText: String,
});
</script>
