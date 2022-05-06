<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script>
import Card from "../../components/Card.vue";

const valkyrie = {
  name: "Miss Pink Elf",
  imageSrc: "/images/miss-pink-elf.png",
  imageAlt: "Miss Pink Elf",
  position: "object-center",
};
</script>