<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "15342a73-c86a-47c9-80dd-b724538ff604",
  name: "Reverist Calico",
  imageSrc: "/images/reverist-calico.jpg",
  imageAlt: "Reverist Calico",
  position: "object-[-8rem]",
};

const signets = {
  builds: [
    {
      name: "Weapon Spam",
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Cat's Eyes",
              desc: "In Runaway state, using Combo ATK/Paw Barrage/Predation increases Total DMG by 10%. It stacks 5 times, and exiting Runaway state removes all stacks",
              priority: "Start",
            },
            {
              name: "Blessing of the Tailpiece",
              desc: "Combo ATK deals 80% more Total DMG. When Combo ATK hits, reduces Megaton Furball's CD by 2s (CD: 5s)",
              priority: "Start",
            },
            {
              name: "Blessing of Hidden Claws",
              desc: "When Combo ATK/Paw Barrage/Predation hits, the target drops 5 Shiny Silvers. It has 5 charges, which reset every floor (unaffected by other effects). It also increases Ice DMG by 45% for 10s. Triggering it again resets the duration",
              priority: "Filler",
            },
            {
              name: "Blessing of Phantasma",
              desc: "Metaton Furball deals 180% more Ice DMG. Runaway state lasts 5s longer",
              priority: "Filler",
            },
            {
              name: "Blessing of Nighteye",
              desc: "Paw Barrage/Predation deals 100% more Total DMG. Using Combo ATK reduces Paw Barrage's CD by 2s",
              priority: "Optional",
            },
          ],
        },
        {
          name: "Vill-V 1",
          lists: [
            {
              name: "Act VI: Sneer",
              desc: "Using a weapon active restores 12 SP in 5s and reduces its CD by 15%",
              priority: "YES",
            },
            {
              name: "Act I: Magic",
              desc: "Using a weapon active boosts its Total DMG by 10%. 6 stacks max. Reset at the end of each battle",
              priority: "1st",
            },
            {
              name: "Act II: Pendulum",
              desc: "Using a weapon active makes enemies take 20% bonus Total DMG for 3.5s. Triggering it again resets the duration",
              priority: "2nd",
            },
            {
              name: "Act IV: Spoon",
              desc: "Using a weapon active boosts Physical DMG and Elemental DMG from Charge ATK and Combo ATK by 25% for 3.5s Triggering it again resets the duration",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Interlude: Reversed Spiral",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Act VIII: Adorned Chamber",
              desc: "Marvellous Magic costs 20 SP to boost its base Physical DMG by 35% and grants 30% Physical Breach for 6s",
              priority: "1st",
            },
          ],
        },
        {
          name: "Kevin 1",
          lists: [
            {
              name: "Artifact of the Inhibitor",
              desc: "Ultimate boosts Elemental Breach by 25% for 5s",
              priority: "1st",
            },
            {
              name: "Brand of the Undead",
              desc: "Ultimate boosts Elemental DMG by 30% for 5s",
              priority: "2nd",
            },
            {
              name: "Goblet of the Giver",
              desc: "Ultimate boosts Total DMG by 35% for 5s",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Blade of the Deliverer",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Crusade of the Deliverer",
              desc: "After 3s into Final Battle, all buffs provided by Normal Signets of Deliverance increase by 90% instead of 50%",
              priority: "1st",
            },
            {
              name: "Echo of the Deliverer",
              desc: "Duration of Final Battle and all buffs provided by Normal Signets of Deliverance are extended to 8s",
              priority: "2nd",
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
              name: "Recitatif of Fruit Tree",
              desc: "The lower the SP. the more SP can be restored from attack (SP regen boost maxed at 100%)",
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
              priority: "1st",
            },
            {
              name: "Echo of Withered Soil",
              desc: "After lasting over 7s, boost SP cap and restore SP/s till it ends",
              priority: "Filler",
            },
          ],
        },
      ],
    },
    {
      name: "Ultimate",
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of the Tailpiece",
              desc: "Combo ATK deals 80% more Total DMG. When Combo ATK hits, reduces Megaton Furball's CD by 2s (CD: 5s)",
              priority: "Start",
            },
            {
              name: "Blessing of Phantasma",
              desc: "Metaton Furball deals 180% more Ice DMG. Runaway state lasts 5s longer",
              priority: "Start",
            },
            {
              name: "Blessing of Cat's Eyes",
              desc: "In Runaway state, using Combo ATK/Paw Barrage/Predation increases Total DMG by 10%. It stacks 5 times, and exiting Runaway state removes all stacks",
              priority: "1st",
            },
            {
              name: "Blessing of Hidden Claws",
              desc: "When Combo ATK/Paw Barrage/Predation hits, the target drops 5 Shiny Silvers. It has 5 charges, which reset every floor (unaffected by other effects). It also increases Ice DMG by 45% for 10s. Triggering it again resets the duration",
              priority: "Filler",
            },
            {
              name: "Blessing of Nighteye",
              desc: "Paw Barrage/Predation deals 100% more Total DMG. Using Combo ATK reduces Paw Barrage's CD by 2s",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Kevin 1",
          lists: [
            {
              name: "Artifact of the Inhibitor",
              desc: "Ultimate boosts Elemental Breach by 25% for 5s",
              priority: "1st",
            },
            {
              name: "Goblet of the Giver",
              desc: "Ultimate boosts Total DMG by 35% for 5s",
              priority: "2nd",
            },
            {
              name: "Rochet of the Pilgrim",
              desc: "Ultimate restores 3 SP per second for 5s",
              priority: "3rd",
            },
            {
              name: "Brand of the Undead",
              desc: "Ultimate boosts Elemental DMG by 30% for 5s",
              priority: "Filler",
            },
            {
              name: "Nexus Signet: Blade of the Deliverer",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Flock of the Deliverer",
              desc: "Final Battle is also considered burst mode. Total DMG increases by 20% in burst mode",
              priority: "1st",
            },
            {
              name: "Echo of the Deliverer",
              desc: "Duration of Final Battle and all buffs provided by Normal Signets of Deliverance are extended to 8s",
              priority: "2nd",
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
              name: "Recitatif of Good Wine",
              desc: "Restore 1.5 SP per second",
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
              priority: "1st",
            },
            {
              name: "Echo of Withered Soil",
              desc: "After lasting over 7s, boost SP cap and restore SP/s till it ends",
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
          ],
        },
        {
          name: "Griseo 1",
          lists: [
            {
              name: "Red & Hot",
              desc: "Using a weapon active taints enemies nearby with red paint for 8s and makes them take 25% bonus Physical and Elemental MG (cannot stack). Triggering it again resets the duration",
              priority: "1st",
            },
            {
              name: "Yellow & Warm",
              desc: "Using an Ultimate taints enemies nearby with yellow paint for 8s and makes them take 30% bonus Total DMG. Triggering it again resets the duration",
              priority: "2nd",
            },
            {
              name: "Grey & Empty",
              desc: "Enemies stay tainted for 5s longer",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Shine like Stars",
              desc: "",
              priority: "CORE",
            },
          ],
        },
        {
          name: "Aponia 1",
          lists: [
            {
              name: "Fourth, No Insolence",
              desc: "Exhortation increases by 5 per second and caps at 200. Ultimate's Physical and Elemental DMG increases by 0.3% of of Exhortation. Using weapon skills reduces 50% Exhortation",
              priority: "1st",
            },
            {
              name: "Sixth, No Decadence",
              desc: "Whenever Exhortation is reduced, enemies take 25% bonus Physical DMG and Elemental DMG for 5s. Can be refreshed",
              priority: "2nd",
            },
          ],
        },
      ],
    },
    {
      name: "Phyllis",
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of the Tailpiece",
              desc: "Combo ATK deals 80% more Total DMG. When Combo ATK hits, reduces Megaton Furball's CD by 2s (CD: 5s)",
              priority: "Start",
            },
            {
              name: "Blessing of Hidden Claws",
              desc: "When Combo ATK/Paw Barrage/Predation hits, the target drops 5 Shiny Silvers. It has 5 charges, which reset every floor (unaffected by other effects). It also increases Ice DMG by 45% for 10s. Triggering it again resets the duration",
              priority: "Start",
            },
            {
              name: "Blessing of Cat's Eyes",
              desc: "In Runaway state, using Combo ATK/Paw Barrage/Predation increases Total DMG by 10%. It stacks 5 times, and exiting Runaway state removes all stacks",
              priority: "1st",
            },
            {
              name: "Blessing of Phantasma",
              desc: "Metaton Furball deals 180% more Ice DMG. Runaway state lasts 5s longer",
              priority: "Filler",
            },
            {
              name: "Blessing of Nighteye",
              desc: "Paw Barrage/Predation deals 100% more Total DMG. Using Combo ATK reduces Paw Barrage's CD by 2s",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Kevin 1",
          lists: [
            {
              name: "Artifact of the Inhibitor",
              desc: "Ultimate boosts Elemental Breach by 25% for 5s",
              priority: "1st",
            },
            {
              name: "Brand of the Undead",
              desc: "Ultimate boosts Elemental DMG by 30% for 5s",
              priority: "2nd",
            },
            {
              name: "Goblet of the Giver",
              desc: "Ultimate boosts Total DMG by 35% for 5s",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Blade of the Deliverer",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Crusade of the Deliverer",
              desc: "After 3s into Final Battle, all buffs provided by Normal Signets of Deliverance increase by 90% instead of 50%",
              priority: "1st",
            },
            {
              name: "Echo of the Deliverer",
              desc: "Duration of Final Battle and all buffs provided by Normal Signets of Deliverance are extended to 8s",
              priority: "2nd",
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
              name: "Recitatif of Fruit Tree",
              desc: "The lower the SP. the more SP can be restored from attack (SP regen boost maxed at 100%)",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Echo of Gold",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Echo of Withered Soil",
              desc: "After lasting over 7s, boost SP cap and restore SP/s till it ends",
              priority: "YES",
            },
            {
              name: "Echo of Silent Night",
              desc: "After lasting over 7s, reduce ATK, DEF, ele resists of enemies nearby",
              priority: "1st",
            },
          ],
        },
        {
          name: "Kalpas 2",
          lists: [
            {
              name: "Bone, Blood, and Ribbon",
              desc: "Every 100 HP loss boosts Physical & Elemental DMG by 0.8%",
              priority: "1st",
            },
            {
              name: "Blade, Grave, and Scar",
              desc: "Every 100 HP loss boosts Total DMG by 1%",
              priority: "2nd",
            },
            {
              name: "Path, Misfortune, and Written Fate",
              desc: "Max HP increases by 25%",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Soldiers, Scissors, Spoils, and Slaughter",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Hometown, Homeland, Friends, and Acquaintances",
              desc: "If [Bloodboil Garment] exceeds 1500, gain 25% physical and elemental breach",
              priority: "1st",
            },
          ],
        },
      ],
    },
  ],
};
</script>