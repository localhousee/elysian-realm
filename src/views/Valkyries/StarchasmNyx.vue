<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script>
import Card from "../../components/Card.vue";

const valkyrie = {
  name: "Starchasm Nyx",
  imageSrc: "/images/starchasm-nyx.png",
  imageAlt: "Starchasm Nyx",
  position: "object-[-4rem]",
};
</script>