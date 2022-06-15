<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "f485ba64-cf4d-4729-8c72-834b173e27b0",
  name: "Fervent Tempo",
  imageSrc: "/images/fervent-tempo.png",
  imageAlt: "Fervent Tempo",
  position: "object-right",
  derp: {
    imageSrc: "/images/derp/fervent-tempo.jpg",
    imageAlt: "Derp Fervent Tempo",
    position: "object-center",
  }
};

const signets = {
  builds: [
    {
      name: "Recommendation",
      supports: [
        {
          time: "",
          sigils: "kevin skill",
          support_1: "SA",
          support_2: "SS",
        },
        {
          time: "Mid",
          sigils: "eden skill",
          support_1: "BR",
          support_2: "SS",
        },
        {
          time: "Late",
          sigils: "eden skill",
          support_1: "SA/BR",
          support_2: "SS",
          recommend: "SA for husk,BR for HoDom",
          Boss: "Möbius FT have type advantage",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "?",
              desc: "Ult CD reduced by 35% (50%) and ult phys dmg increased 300% (400%), when ult deals dmg reduce weapon active cd by 2s, retaliation trigger time frame is increased to entire defending duration",
              priority: "Start",
            },
            {
              name: "?",
              desc: "Normal attacks (and charged attacks) deal 30% (50%) more phys dmg and every hit recovers 1 more SP, when SP exceeds 150 doubles ult SP cost and dmg, in ult duration enemies take 30% (50%) more TDM",
              priority: "1st",
            },
            {
              name: "?",
              desc: "Fervent Mode normal attacks deal 30% (40%) additional phys dmg. Final hit of ultimate deals additional 400% (600%) phys dmg",
              priority: "2nd",
            },
          ],
        },
        {
          name: "Eden 2",
          lists: [
            {
              name: "Recitatif of Fine Jade",
              desc: "Initial SP and max SP increase by 30",
              priority: "1st",
            },
            {
              name: "Recitatif of Creeks",
              desc: "Every 10 SP left boosts Physical & Elemental DMG by 2.5%",
              priority: "2nd",
            },
            {
              name: "Recitatif of Good Wine",
              desc: "Restore 1.5 SP per second",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Echo of Gold",
              desc: "Consuming SP restores the same charges and triggers Final Echo status during which Total DMG increases 8% (160% max) at the cost of charges equal to the remaining duration per second. Insufficient charges reset the effect and end Final Echo",
              priority: "CORE",
            },
          ],
        },
        {
          name: "Kevin 1",
          lists: [
            {
              name: "Mask of the Predator",
              desc: "Ultimate boosts Physical Breach by 25% for 5s",
              priority: "1st",
            },
            {
              name: "Pendant of the Watcher",
              desc: "Ultimate boosts Physical DMG by 30% for 5s",
              priority: "2nd",
            },
            {
              name: "Goblet of the Giver",
              desc: "Ultimate boosts Total DMG by 35% for 5s",
              priority: "3rd",
            },
            {
              name: "Rochet of the Pilgrim",
              desc: "Ultimate restores 3 SP per second for 5s",
              priority: "4th",
            },
            {
              name: "Nexus Signet: Blade of the Deliverer",
              desc: "Ultimate triggers Final Battle status during which all buffs provided by Normal Signets of Deliverance increase by for 5s",
              priority: "CORE",
            },
            {
              name: "Echo of the Deliverer",
              desc: "Duration of Final Battle and all buffs provided by Normal Signets of Deliverance are extended to 8s",
              priority: "1st",
            },
            {
              name: "Crusade of the Deliverer",
              desc: "After 3s into Final Battle, all buffs provided by Normal Signets of Deliverance increase by 90% instead of 50%",
              priority: "2nd",
            },
          ],
        },
        {
          name: "Griseo 2",
          lists: [
            {
              name: "Yellow & Warm",
              desc: "Using an Ultimate taints enemies nearby with yellow paint for 8s and makes them take 30% bonus Total DMG. Triggering it again resets the duration",
              priority: "1st",
            },
            {
              name: "Red & Hot",
              desc: "Using a weapon active taints enemies nearby with red paint for 8s and makes them take 25% bonus Physical and Elemental DMG (cannot stack). Triggering it again resets the duration",
              priority: "2nd",
            },
            {
              name: "Black & Dark",
              desc: "Every time an enemy is tainted, Valkyries deals 10% bonus Physical and Elemental DMG for 20s. 6 stacks max",
              priority: "3rd",
            },
            {
              name: "White & Bright",
              desc: "Every time an enemy is tainted, Valkyrie restores 12 SP. CD: 5s",
              priority: "4th",
            },
            {
              name: "Nexus Signet: ?",
              desc: "?",
              priority: "CORE",
            },
          ],
        },
      ],
    },
  ],
};
</script>
