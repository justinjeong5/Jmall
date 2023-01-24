<script setup>
import { ref } from "vue";
import api from "@lib/api.js";

defineProps({
    msg: String,
});

api

const count = ref(0);
</script>

<template>
    <h1>{{ msg }}</h1>
    <v-alert closable
             icon="mdi-vuetify"
             title="Alert title"
             text="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing">
    </v-alert>
</template>

<style scoped>
.read-the-docs {
    color: #888;
}
</style>
