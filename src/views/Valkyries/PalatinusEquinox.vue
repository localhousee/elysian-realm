<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "9be32ce4-b6e8-4237-bf4d-e091f2d8ee4d",
  name: "Palatinus Equinox",
  imageSrc: "/images/palatinus-equinox.jpg",
  imageAlt: "Palatinus Equinox",
  position: "object-top",
};

const signets = {
  builds: [
    {
      name: "Recommendation",
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "VC",
          support_2: "BR",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "VC",
          support_2: "BR",
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
              name: "Blessing of Gallop",
              desc: "Consumes Knight Guardian to restore all ICHOR",
              priority: "Start",
            },
            {
              name: "Blessing of Abyssal Chant",
              desc: "Ultimate Evasion skill refreshed twice after casting Ultimate",
              priority: "1st",
            },
            {
              name: "Blessing of Equinox",
              desc: "Palatinus Equinox is enhanced when switching forms and using Ultimate",
              priority: "2nd",
            },
            {
              name: "Blessing of Commitment",
              desc: "Increases Total DMG of weapon skills",
              priority: "No",
            },
            {
              name: "Blessing of Exodus",
              desc: "Last hit of Equinox Severance consumes Knight Guardian and impairs enemies",
              priority: "No",
            },
          ],
        },
        {
          name: "Sakura 1 (Choose one)",
          lists: [
            {
              name: "Bountiful Blossom: Koyo",
              desc: "Triggering Ultimate Evasion Skill boosts Total DMG taken by all enemies by 30% for 8s",
              priority: "1st",
            },
            {
              name: "Bountiful Blossom: Ayame",
              desc: "Triggering Ultimate Evasion Skill restores 12.0 bonus SP",
              priority: "2nd",
            },
            {
              name: "Bountiful Blossom: Fuji",
              desc: "Ultimate Evasion Skill has 1 more charge and 10% reduced CD",
              priority: "3rd",
            },
            {
              name: "Nexus Signet Setsuna Blade: Sakura ni Maku",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Setsuna Blade: Ame-Shiko",
              desc: "Activating Sakura Screen resets Ultimate CD and weapon active CD",
              priority: "YES",
            },
          ],
        },
        {
          name: "Sakura 2 (Choose one)",
          lists: [
            {
              name: "Bountiful Blossom: Fuji",
              desc: "Ultimate Evasion Skill has 1 more charge and 10% reduced CD",
              priority: "YES",
            },
            {
              name: "Bountiful Blossom: Ayame",
              desc: "Triggering Ultimate Evasion Skill restores 12.0 bonus SP",
              priority: "1st",
            },
            {
              name: "Bountiful Blossom: Kiku",
              desc: "Ultimate Evasions reset Ultimate Evasion Skill CD",
              priority: "2nd",
            },
            {
              name: "Bountiful Blossom: Koyo",
              desc: "Triggering Ultimate Evasion Skill boosts Total DMG taken by all enemies by 30% for 8s",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Setsuna blade: Yasha",
              desc: "",
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
              desc: "Every 100 HP loss boosts Total DMG by 1%",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Soldiers, Scissors, Spoils, and Slaughter",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Death, Life, Oblivion, and Existence",
              desc: "If [Bloodboil Garment] exceeds 1500, when taking damage, reduces damage taken by 1% of [Bloodboil Garment]",
              priority: "Filler",
            },
          ],
        },
      ],
    },
  ],
};
</script>