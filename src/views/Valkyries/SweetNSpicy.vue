<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "d5f90693-c493-4f05-9c1a-183e30e617fc",
  name: "Sweet N Spicy",
  imageSrc: "/images/sweet-n-spicy.jpg",
  imageAlt: "Sweet N Spicy",
  position: "object-[-3rem]",
};

const signets = {
  builds: [
    {
      name: "Recommendation",
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "SS",
          support_2: "VC",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "SS",
          support_2: "VC / BR",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "SS",
          support_2: "BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Revolution",
              desc: "Each charging stage reduces Ultimate CD by 0.8s. Ultimate and aerial Charged ATK deal 10% bonus Physical DMG to enemies not protected by shields",
              priority: "Start",
            },
            {
              name: "Blessing of Skyfall",
              desc: "Each stage of aerial charging stacks Momentum once up to 6 stacks. Each stack boosts Ultimate DMG by 15%. Removed upon Ultimate cast",
              priority: "1st",
            },
            {
              name: "Blessing of Impulse",
              desc: "Armor Shredder maxes at 4 stacks and stacks twice each time",
              priority: "No",
            },
            {
              name: "Blessing of Brake",
              desc: "Charging speed accelerates and Physical DMG of Charged ATK increases by 10%. My Hands Are Burning stacks faster",
              priority: "No",
            },
            {
              name: "Blessing of Rupture",
              desc: "Ground Charged ATK can charge up to 4 stages and deal 400% ATK of bonus Physical DMG",
              priority: "No",
            },
          ],
        },
        {
          name: "Kosma 1",
          lists: [
            {
              name: "Eyes that Overlook the Vicious Abyss",
              desc: "Each stack of Rend on enemies makes Valkyries deal 10% bonus DMG to their shields",
              priority: "YES",
            },
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
              name: "Wings that Mask the Sanguine Moon",
              desc: "Ultimate Evasion Skill inflicts 8 stacks of Rend on all enemies, each stack dealing 20% ATK of Adaptive DMG per second for 70s. 10 stacks max. CD: 8s",
              priority: "Filler",
            },
            {
              name: "Breath that Slanders Sulphur",
              desc: "Inflicting Rend on an already affected enemy restores 10 SP. CD: 5s",
              priority: "Filler",
            },
            {
              name: "Nexus Signet: Daybreak, an Undying Light",
              desc: "",
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
              desc: "",
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
          name: "Kalpas 2",
          lists: [
            {
              name: "Path, Misfortune, and Written Fate",
              desc: "Max HP increases by 25%",
              priority: "1st",
            },
            {
              name: "Bone, Blood, and Ribbon",
              desc: "Every 100 HP loss boosts Physical & Elemental DMG by 0.8%",
              priority: "2nd",
            },
            {
              name: "Blade, Grave, and Scar",
              desc: "Every 100 HP loss boosts Total DMG by 1.0%",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Soldiers, Scissors, Spoils, and Slaughter",
              desc: "HP cannot exceed 18% of max HP. Healing HP charges [Bloodboil Garment]",
              priority: "CORE",
            },
            {
              name: "Death, Life, Oblivion, and Existence",
              desc: "If [Bloodboil Garment] exceeds 1500, when taking damage, reduces damage taken by 1% of [Bloodboil Garment]",
              priority: "YES",
            },
          ],
        },
      ],
    },
  ],
};
</script>