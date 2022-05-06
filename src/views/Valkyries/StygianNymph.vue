<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script>
import Card from "../../components/Card.vue";

const valkyrie = {
  name: "Stygian Nymph",
  imageSrc: "/images/stygian-nymph.jpg",
  imageAlt: "Stygian Nymph",
  position: "object-center",
};
</script>