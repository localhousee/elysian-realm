<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "d218fff3-9947-40d9-9f6e-7eb14badfe33",
  name: "Starry Impression",
  imageSrc: "/images/starry-impression.jpg",
  imageAlt: "Starry Impression",
  position: "object-left",
  derp: {
    imageSrc: "/images/starry-impression.jpg",
    imageAlt: "Derp Starry Impression",
    position: "object-center",
  }
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
        {
          name: "Elysia",
          lists: [
            {
              name: "?",
              desc: "For every stack of bleed on enemies, gain Total DMG +8/10%. When using combo attack to consume all 3 colors, deal an additional 800/1000%ATK Physical Bleed damage, CD 0.5s",
              priority: "Start",
            },
            {
              name: "?",
              desc: "When activating ultimate evasion, gain 3 different ink colors and make all enemies on field take 30/40% more TDM for 10s",
              priority: "1st",
            },
            {
              name: "?",
              desc: "Physical DMG 30/40%. Normal attack sequence 4 gathers enemies",
              priority: "2nd",
            },
            {
              name: "?",
              desc: "Combo ATK deals an additional 100/200% 1000/2000% 1000/1200% ATK Physical DMG for each color consumed. When consuming red/yellow/blue color, reduce weapon active/ultimate/evasion CD by 1s respectively. Combo attack that consumes all colors can also chain to 3rd sequence of normal attack",
              priority: "2nd",
            },
            {
              name: "?",
              desc: "During ultimate, gain +25% attack speed and 3rd/5th sequence of normal attack grant an additional color (same as normal attack color). During ultimate, all enemies take 10/20% more Total DMG (independent effect)",
              priority: "No",
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
              name: "Red & Hot",
              desc: "Using a weapon active taints enemies nearby with red paint for 8s and makes them take 25% bonus Physical and Elemental MG (cannot stack). Triggering it again resets the duration",
              priority: "1st",
            },
            {
              name: "Black & Dark",
              desc: "Every time an enemy is tainted, Valkyries deals 10% bonus Physical and Elemental DMG for 20s. 6 stacks max",
              priority: "2nd",
            },
              {
                name: "Yellow & Warm",
                desc: "Using an Ultimate taints enemies nearby with yellow paint for 8s and makes them take 30% bonus Total DMG. Triggering it again resets the duration",
                priority: "3rd",
              },
            {
              name: "White & Bright",
              desc: "Every time an enemy is tainted, Valkyrie restores 12 SP. CD: 5s",
              priority: "4th",
            },
            {
              name: "Nexus Signet: Dim like Stars",
              desc: "",
              priority: "CORE",
            },
          ],
        },
        {
          name: "Kosma 1",
          lists: [
            {
              name: "Talons that Desecrate the Santuary",
              desc: "Basic/Combo/Charged ATKs inflict a stack of Rend on hit, each stack dealing 20% ATK of Adaptive DMG per second for 10s. 70 stacks max. Stacking CD: 1s",
              priority: "1st",
            },
            {
              name: "Horns that Rip the Bleak Sky",
              desc: "Ultimate inflicts 8 stacks of Rend on all enemies, each stack dealing 20% ATK of Adaptive DMG per second for 10s. 70 stacks max. CD: 8s",
              priority: "2nd",
            },
            {
              name: "Heart that Committed Seven Crimes",
              desc: "Rend lasts 5s longer",
              priority: "3rd",
            },
            {
              name: "Breath that Slanders Sulphur",
              desc: "Inflicting Rend on an already affected enemy restores 10 SP. CD: 5s",
              priority: "Filler",
            },
            {
              name: "Nexus Signet: Daybreak, an Undying Light",
              desc: "Hitting an enemy with 10 or more stacks of Rend triggers Evil's Doom which deals ATK of Adaptive 1500% DMG and 5000% ATK of bonus Adaptive DMG against shields. CD: 5s",
              priority: "CORE",
            },
            {
              name: "Unwavering Promise",
              desc: "Rend-inflicted enemies take 80% bonus Total DMG and addition 40% bonus Total DMG with 20 Rend stacks or more",
              priority: "Filler",
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
              name: "Recitatif of Eden",
              desc: "Every 10 SP left boosts Total DMG by 3.0%",
              priority: "2nd",
            },
            {
              name: "Recitatif of Fine Jade",
              desc: "Initial SP and max SP increase by 30",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Echo of Gold",
              desc: "Consuming SP restores the same charges and triggers Final Echo status during which Total DMG increases 8% (160% max) at the cost of charges equal to the remaining duration per second. Insufficient charges reset the effect and end Final Echo",
              priority: "CORE",
            },
          ],
        },
       ],
     },
   ],
};
</script>
