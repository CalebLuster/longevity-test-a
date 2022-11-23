<script lang="ts" setup>
import ChipCard from "./ChipCard.vue";
  const cards = [
        {
          id: 0,
          title: "Depersonalization API",
          content:
            "Remove information that can identify patients Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit. Exercitation veniam consequat sunt nostrud amet.",
        },
        {
          id: 1,
          title: "Prediction API",
          content:
            "Feed depersonalized data to predict if your patient has the chance of encountering a disease ",
        },
        {
          id: 2,
          title: "Custom Prediction Models",
          content:
            "Create or import your own models to quickly run checkups with data yur patients share with you",
        },
        {
          id: 3,
          title: "Document analysis",
          content:
            "Extract information from clinical tests by scanning images, PDFs and spreadsheets ",
        },
        {
          id: 4,
          title: "Data Structuring",
          content:
            "Using the data you send, we return a structure in a standard format easy to convert and integrate to other formats",
        },
      ]
</script>

<template>
  <div>
    <ChipCard title="Depersonalization" :items="cards" href="" />
  </div>
</template>

<style></style>
