<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "0ada4055-07cc-46b5-9ddc-4fa4c65e1edb",
  name: "Fallen Rosemary",
  imageSrc: "/images/fallen-rosemary.jpg",
  imageAlt: "Fallen Rosemary",
  position: "object-center",
};

const signets = {
  builds: [
    {
      name: "Recommendation",
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "AE",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "AE",
          support_2: "LE / BR",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "AE",
          support_2: "BR",
        },
      ],
      signets: [
        {
          name: "Elysia, rank < SS2",
          lists: [
            {
              name: "Blessing of Nocturne",
              desc: "Using God Eater increases Charge ATK TDM",
              priority: "Start",
            },
            {
              name: "Blessing of Soul Siphon",
              desc: "In Valfreyja form basic ATK siphons extra Disir",
              priority: "1st",
            },
            {
              name: "Blessing of Valfreyja",
              desc: "In Valfreyja form Lightning DMG is increased",
              priority: "2nd",
            },
            {
              name: "Blessing of God Eater",
              desc: "When God Eater hits, a lightning bolt hits and fully recharges Strix",
              priority: "Filler",
            },
            {
              name: "Blessing of Spirit Servants",
              desc: "When Garmr/Strix/Linnorm hits, increases Lightning DMG",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Elysia, rank >= SS2",
          lists: [
            {
              name: "Blessing of Nocturne",
              desc: "Using God Eater increases Charge ATK TDM",
              priority: "Start",
            },
            {
              name: "Blessing of Valfreyja",
              desc: "In Valfreyja form Lightning DMG is increased",
              priority: "1st",
            },
            {
              name: "Blessing of God Eater",
              desc: "When God Eater hits, a lightning bolt hits and fully recharges Strix",
              priority: "2nd",
            },
            {
              name: "Blessing of Soul Siphon",
              desc: "In Valfreyja form basic ATK siphons extra Disir",
              priority: "3rd",
            },
            {
              name: "Blessing of Spirit Servants",
              desc: "When Garmr/Strix/Linnorm hits, increases Lightning DMG",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Su 2",
          lists: [
            {
              name: "Motto of Dibba-Cakkhu",
              desc: "Combo hits are reset at to boost Total DMG taken by all enemies by 35% for 10s",
              priority: "1st",
            },
            {
              name: "Motto of Asavakkhaya",
              desc: "Attacks grant 25 bonus combo hits on hit. CD: 5s",
              priority: "2nd",
            },
            {
              name: "Motto of Iddhi-Vidha",
              desc: "Combo hits are increased to 60 when below 60. CD: 10s",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Dictum of Bodhi",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Dictum of Anatman",
              desc: "The Bodhi: Eyes Open lasts for 3s longer. For every debuff on the target enemy, it takes 5% bonus Total DMG",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Kevin 1",
          lists: [
            {
              name: "Artifact of the Inhibitor",
              desc: "Ultimate boosts Elemental Breach by 20% for 5s",
              priority: "1st",
            },
            {
              name: "Brand of the Undead",
              desc: "Ultimate boosts Elemental DMG by 30% for 5s",
              priority: "2nd",
            },
            {
              name: "Rochet of the Pilgrim",
              desc: "Ultimate restores 3 SP per second for 5s",
              priority: "3rd",
            },
            {
              name: "Goblet of the Giver",
              desc: "Ultimate boosts Total DMG by 35% for 5s",
              priority: "Filler",
            },
            {
              name: "Nexus Signet: Blade of the Deliverer",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Crusade of the Deliverer",
              desc: "After 3s into Final Battle, all buffs provided by Normal Signets of Deliverance increase by 90% instead of 50%",
              priority: "YES",
            },
            {
              name: "Echo of the Deliverer",
              desc: "Duration of Final Battle and all buffs provided by Normal Signets of Deliverance are extended to 8s",
              priority: "1st",
            },
          ],
        },
        {
          name: "Eden 2",
          lists: [
            {
              name: "Recitatif of Creeks",
              desc: "Every 10 SP left boosts Physical & Elemental DMG by 2.5%",
              priority: "1st",
            },
            {
              name: "Recitatif of Fine Jade",
              desc: "Initial SP and max SP increase by 30",
              priority: "2nd",
            },
            {
              name: "Recitatif of Birds",
              desc: "Every 10 SP left reduces Total DMG taken by 2.5%",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Echo of Gold",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Echo of Silent Night",
              desc: "After lasting over 7s, reduce ATK, DEF, ele resists of enemies nearby",
              priority: "YES",
            },
          ],
        },
      ],
    },
  ],
};
</script>
