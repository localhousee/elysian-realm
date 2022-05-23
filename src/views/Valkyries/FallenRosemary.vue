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
  position: "object-top",
  derp: {
    imageSrc: "/images/derp/fallen-rosemary.jpg",
    imageAlt: "Derp Fallen Rosemary",
    position: "object-center",
  }
};

const signets = {
  builds: [
    {
      name: "Recommendation",
      supports: [
        {
          time: "Early",
          sigils: "Burden",
          support_1: "AE",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "Light as a Bodhi Leaf/Gold Goblet",
          support_1: "AE",
          support_2: "LE / BR",
        },
        {
          time: "Late",
          sigils: "Dreamful Gold/Home Lost",
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
          info: "The loop-able combo from Soul Siphon drops from being used 6 times to 3 times at SS2",
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
              desc: "Reaching 60/100/150 combo hits unleashes Bodhi: Eyes Open on a random enemy, dealing 800%/900%/1000% ATK of adaptive DMG and inflicting Trance. Affected enemies contribute 1 bonus combo hit on hit for 3s",
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
              desc: "Ultimate triggers Final Battle status during which all buffs provided by Normal Signets of Deliverance increase by for 5s",
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
              desc: "Consuming SP restores the same charges and triggers Final Echo status during which Total DMG increases 8% (160% max) at the cost of charges equal to the remaining duration per second. Insufficient charges reset the effect and end Final Echo",
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
