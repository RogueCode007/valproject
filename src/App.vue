<script setup>
import ThanksPage from "./components/ThanksPage.vue";
import Question from "./components/Question.vue";
import { ref } from "vue";

const chosenYes = ref(false);
</script>

<template>
  <Question v-if="!chosenYes" @choose-yes="chosenYes = true" />
  <ThanksPage v-else />
</template>
