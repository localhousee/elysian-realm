<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  name: "Herrscher Of Reason",
  imageSrc: "/images/herrscher-of-reason.jpg",
  imageAlt: "Herrscher Of Reason",
  position: "object-center",
};

const signets = {
  builds: [
    {
      name: "Evade",
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "AE",
          support_2: "HB / BR",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "AE",
          support_2: "HB / BR",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "AE",
          support_2: "HB / BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Truth",
              desc: "Triggering Ultimate Evasion Skill fully restores Konstruktyom. When Konstruktyom is below 120, any evasion can trigger Ultimate Evasion Skill",
              priority: "Start",
            },
            {
              name: "Blessing of Inspiration",
              desc: "Triggering an Ultimate Evasion by any means inflicts a Structural Impact on enemies hit and deals 3750% ATK of Ice DMG",
              priority: "1st",
            },
            {
              name: "Blessing of Reason",
              desc: "Every hit from hover guns reduces weapon active CD by 0.7s",
              priority: "2nd",
            },
            {
              name: "Blessing of Creation",
              desc: "In non-bike mode, Charged ATKs create 4 hover guns to attack, each dealing 160% ATK of Ice DMG on hit",
              priority: "Filler",
            },
            {
              name: "Blessing of Wisdom",
              desc: "In bike mode, Charged ATK inflicts a Structural Impact on enemies hit and deals 2250% ATK of Ice DMG",
              priority: "No",
            },
          ],
        },
        {
          name: "Sakura 2",
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
              name: "Blue & Cold",
              desc: "Triggering an Ultimate Evasion Skill taints enemies nearby with blue paint for 8s and reduces their Total DMG and Move Speed by 30%. Triggering it again resets the duration",
              priority: "4th",
            },
            {
              name: "Nexus Signet: Shine like Stars",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Blooming like Flowers",
              desc: "When enemies of countering types are tainted with both blue and red paints, Valkyries deal 50% bonus Total DMG to them (cannot stack)",
              priority: "YES",
            },
          ],
        },
        {
          name: "Hua 2",
          lists: [
            {
              name: "Old Dreams Again",
              desc: "Elemental Breach increases by 0.6% per second",
              priority: "1st",
            },
            {
              name: "Dark Garb No More",
              desc: "Elemental DMG increases by 0.8% per second",
              priority: "2nd",
            },
            {
              name: "Lost and Found",
              desc: "Total DMG taken decreases by 0.8% per second",
            },
            {
              name: "Nexus Signet: Suffering Mass",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Worldly Troubles",
              desc: "With Soldier's Remembrance, gain TDM equal to 50% of total damage reduction from signets",
              priority: "1st",
            },
            {
              name: "Broken Dream",
              desc: "When possessing Soldier's Remembrance, increase the maximum stack of normal Vicissitude signets by 20",
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
      ],
    },
    {
      name: "Ultimate",
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "AE",
          support_2: "HB / BR",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "AE",
          support_2: "LE / HB / BR",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "AE",
          support_2: "HB / BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Truth",
              desc: "Triggering Ultimate Evasion Skill fully restores Konstruktyom. When Konstruktyom is below 120, any evasion can trigger Ultimate Evasion Skill",
              priority: "Start",
            },
            {
              name: "Blessing of Inspiration",
              desc: "Triggering an Ultimate Evasion by any means inflicts a Structural Impact on enemies hit and deals 3750% ATK of Ice DMG",
              priority: "1st",
            },
            {
              name: "Blessing of Wisdom",
              desc: "In bike mode, Charged ATK inflicts a Structural Impact on enemies hit and deals 2250% ATK of Ice DMG",
              priority: "2nd",
            },
            {
              name: "Blessing of Reason",
              desc: "Every hit from hover guns reduces weapon active CD by 0.7s",
              priority: "3rd",
            },
            {
              name: "Blessing of Creation",
              desc: "In non-bike mode, Charged ATKs create 4 hover guns to attack, each dealing 160% ATK of Ice DMG on hit",
              priority: "No",
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
              name: "Blue & Cold",
              desc: "Triggering an Ultimate Evasion Skill taints enemies nearby with blue paint for 8s and reduces their Total DMG and Move Speed by 30%. Triggering it again resets the duration",
              priority: "4th",
            },
            {
              name: "Nexus Signet: Shine like Stars",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Blooming like Flowers",
              desc: "When enemies of countering types are tainted with both blue and red paints, Valkyries deal 50% bonus Total DMG to them (cannot stack)",
              priority: "YES",
            },
          ],
        },
        {
          name: "Kevin 2",
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
              name: "Nexus Signet: Shadow of the Deliverer",
              desc: "",
              priority: "CORE",
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
              desc: "After lasting over 7s in Final Note, reduce ATK, DEF, ele resists of enemies nearby",
              priority: "1st",
            },
            {
              name: "Echo of Withered Soil",
              desc: "After lasting over 7s in Final Note, boost SP cap and restore SP/s till it ends",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Sakura 1",
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
      ],
    },
  ],
};
</script>