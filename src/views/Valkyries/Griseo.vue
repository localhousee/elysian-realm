<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "d218fff3-9947-40d9-9f6e-7eb14badfe33",
  name: "Griseo",
  imageSrc: "/images/griseo.jpg",
  imageAlt: "Griseo",
  position: "object-left",
};

const signets = {
builds: [
     {
       name: "Omni Ego",
       supports: [
         {
           time: "Early",
           sigils: "Because of You",
           support_1: "",
           support_2: "",
         },
         {
           time: "Mid",
           sigils: "",
           support_1: "",
           support_2: "SA",
         },
         {
           time: "Late",
           sigils: "Dreamful Gold",
           support_1: "SS",
           support_2: "SA",
         },
       ],
       signets: [
       ],
     },
   ],
};
</script>
