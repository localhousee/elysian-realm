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
      name: "Recommendation",
      boss: "Aponia",
      recommended: "",
      supports: [
        {
          time: "Early",
          sigils: "Because of You / It will be Written",
          support_1: "SA",
          support_2: "SS",
        },
        {
          time: "Mid",
          sigils: "Dreamful Gold",
          support_1: "BR",
          support_2: "SS",
        },
        {
          time: "Late",
          sigils: "Dreamful Gold",
          support_1: "SS",
          support_2: "SA / BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Feathers",
              desc: "Total DMG dealt to enemies inflicted with Bleed increases 8% for every stack inflicted. Combo ATKs grant buffs upon consuming all Color Markers and deal 800% ATK of Bleed DMG on hit. CD: 0.5s",
              priority: "Start",
            },
            {
              name: "Blessing of Azure Wind",
              desc: "Triggering Ultimate Evasion Skill grants 3 Color Markers and boosts Total DMG taken by all enemies by 40% for 20s",
              priority: "1st",
            },
            {
              name: "Blessing of Cloud Valley",
              desc: "Physical DMG increases 40% and SEQ 4 of Basic ATKs draw in surrounding enemies within a wide radius",
              priority: "2nd",
            },
            {
              name: "Blessing of Starry Night",
              desc: "Combo ATKs deal an additional 1000% ATK Physical DMG for every Color Marker consumed. This DMG counts as bleeding DMG. Upon consuming Red, Yellow, or Blue Color Marker, Valkyrie's Weapon Skill, Ultimate, and Ultimate Evasion CDs are reduced 1s. Combo ATKs consuming all Color Markers can be connected into Basic ATK SEQ 3",
              priority: "2nd",
            },
            {
              name: "Blessing of River Forest",
              desc: "Valkyrie's ATK Speed increases 25% during Ultimate, and SEQ 3 and SEQ 5 of Basic ATKs gain an additional Color Markers (samecolor as would be normally granted). DMG dealt to all enemies during Ultimate increases 10% (cannot stack)",
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
