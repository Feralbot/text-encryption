<template>
  <v-app class="bg-grey-darken-2">
    <v-container>
      <HeaderComp />
      <v-main class="d-flex flex-column mb-6 justify-space-evenly">
        <TextOutput :InputedText="InputedText" />
        <LoadSaveBtns />
        <TextInput v-model="InputedText" />
      </v-main>
    </v-container>
  </v-app>
</template>

<script setup>
import HeaderComp from "./components/HeaderComp.vue";
import TextOutput from "./components/TextOutput.vue";
import LoadSaveBtns from "./components/LoadSaveBtns.vue";
import TextInput from "./components/TextInput.vue";
import { ref } from "vue";
const InputedText = ref("");
</script>
