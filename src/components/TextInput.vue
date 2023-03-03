<template>
  <v-textarea
    class="rounded-lg"
    color="white"
    v-model="InputedText"
    label="Enter text here"
    @input="$emit('update:modelValue', $event.target.value)"
  >
  </v-textarea>
</template>

<script setup>
import { ref } from "vue";
const InputedText = ref("");
</script>
