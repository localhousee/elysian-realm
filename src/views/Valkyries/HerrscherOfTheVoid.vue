<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "cd05bc6e-018e-482c-9d16-56b239eda0de",
  name: "Herrscher Of The Void",
  imageSrc: "/images/herrscher-of-the-void.png",
  imageAlt: "Herrscher Of The Void",
  position: "object-center",
};

const signets = {};
</script>