<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "9be32ce4-b6e8-4237-bf4d-e091f2d8ee4d",
  name: "Palatinus Equinox",
  imageSrc: "/images/palatinus-equinox.png",
  imageAlt: "Palatinus Equinox",
  position: "object-center",
  derp: {
    imageSrc: "/images/derp/palatinus-equinox.png",
    imageAlt: "Derp Palatinus Equinox",
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
              desc: "Triggering Ultimate Evasion Skill 3 times activates Sakura Screen to render all enemies static for 3s, after which they lose HP equal to 40% of the DMG they have received during the duration",
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
              desc: "Valkyries enter Isshun status every 10s during which a normal evasion becomes Ultimate Evasion and unleashes Setsuna Blade: Karuma dealing 7x200% ATK of Ice DMG to all enemies",
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
          ],
        },
        {
          name: "Kalpas 2",
          lists: [
            {
              name: "Desireless, Mindless, and Homeless",
              desc: "Losing HP boosts Total DMG taken by all enemies by 25% for 8s",
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
              name: "Path, Misfortune, and Written Fate",
              desc: "Max HP increases by 25%",
              priority: "Filler",
            },
            {
              name: "Nexus Signet: Soldiers, Scissors, Spoils, and Slaughter",
              desc: "Valkyrie's current HP cannot exceed 18% of her Max HP, and if the HP recovery in combat reaches 0/400/800, the recovery amount increases by of the Bloodboil Armor charges, up to for a single charge. The charge cap is 1800, and each point increases the HP cap by 1",
              priority: "CORE",
            },
            {
              name: "Death, Life, Oblivion, and Existence",
              desc: "The Bloodboil Armor charges cap increases by 500. At over 1500 charges, Bloodboil Armor can absorb DMG equal to 1% of its charges",
              priority: "Filler",
            },
          ],
        },
      ],
    },
  ],
};
</script>
