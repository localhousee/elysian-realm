<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "ca2fc0d6-2ea0-41c9-96d5-1b7c7ae5a144",
  name: "Midnight Absinthe",
  imageSrc: "/images/midnight-absinthe.jpg",
  imageAlt: "Midnight Absinthe",
  position: "object-left",
  derp: {
    imageSrc: "/images/derp/midnight-absinthe.png",
    imageAlt: "Derp Midnight Absinthe",
    position: "object-center",
  }
};

const signets = {
  builds: [
    {
      name: "5 Core",
      recommended: "HoD",
      boss: "",
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
          support_2: "LE / MA / BR",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "AE",
          support_2: "MA / BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Ominous Mist",
              desc: "Raven Cloud has a large range and deals 6500% DMG when it explodes. Raven Cloud vaporizes after the explosion",
              priority: "Start",
            },
            {
              name: "Blessing of Arrowhead",
              desc: "Weapon actives restore 24 bonus SP and reduce Ultimate CD by 10s. Can only be triggered once per 8s",
              priority: "1st",
            },
            {
              name: "Blessing of Wild Hunt",
              desc: "The follow-up of Basic ATK Sequence 5 is no longer limited by Night Roamer stacks. Basic ATK Sequence 5 and every hit of the follow-up consume 10 Night Roamer stacks to shoot 5 more arrows, each dealing 150% ATK of Fire DMG",
              priority: "Filler",
            },
            {
              name: "Blessing of Suppression",
              desc: "Feather Arrows, Feather Blades, Feathers, and Night Roamer stacks cap at 30. Night Roamer boosts Fire DMG by 15%",
              priority: "Filler",
            },
            {
              name: "Blessing of Raven Plume",
              desc: "Ultimate Evasion Skill reduces the ATK of enemies nearby by 60% and makes Valkyrie's attacks deal 25% ATK of bonus Fire DMG for 12s. Ultimate Evasion Skill has one extra charge",
              priority: "No",
            },
          ],
        },
        {
          name: "Vill-V 1",
          lists: [
            {
              name: "Act II: Pendulum",
              desc: "Using a weapon active makes enemies take 20% bonus Total DMG for 3.5s. Triggering it again resets the duration",
              priority: "1st",
            },
            {
              name: "Act VI: Sneer",
              desc: "Using a weapon active restores 12 SP in 5s and reduces its CD by 15%",
              priority: "2nd",
            },
            {
              name: "Act V: Spider Web",
              desc: "Using a weapon active boosts Valkyrie ranged Total DMG by 40% for 3.5s. Triggering it again resets the duration",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Interlude: Reversed Spiral",
              desc: "Using a weapon active unleashes Marvellous Magic dealing 3x400% ATK of Physical DMG to enemies in front and making them take 25% bonus Total DMG for 8s. CDL 5s. The DMG is guaranteed to Crit and the weapon active is the DMG source",
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
              desc: "Ultimate boosts Elemental Breach by 20% for 5s",
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
              desc: "Ultimate triggers Final Battle status during which all buffs provided by Normal Signets of Deliverance increase by for 5s",
              priority: "CORE",
            },
            {
              name: "Echo of the Deliverer",
              desc: "Duration of Final Battle and all buffs provided by Normal Signets of Deliverance are extended to 8s",
              priority: "YES",
            },
            {
              name: "Crusade of the Deliverer",
              desc: "After 3s into Final Battle, all buffs provided by Normal Signets of Deliverance increase by 90% instead of 50%",
              priority: "YES",
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
              priority: "4th / Filler",
            },
            {
              name: "Nexus Signet: Shine like Stars",
              desc: "When there are enemies tainted with 1/2/3 different paints, Valkyries deal 20%/50%/100% bonus Total DMG to enemies of countering types",
              priority: "CORE",
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
              priority: "Optional",
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
              name: "Recitatif of Good Wine",
              desc: "Restore 1.5 SP per second",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Echo of Gold",
              desc: "Consuming SP restores the same charges and triggers Final Echo status during which Total DMG increases 8% (160% max) at the cost of charges equal to the remaining duration per second. Insufficient charges reset the effect and end Final Echo",
              priority: "CORE",
            },
            {
              name: "Echo of Silent Night",
              desc: "After lasting over 7s in Final Note, reduce ATK, DEF, ele resists of enemies nearby",
              priority: "1st",
            },
          ],
        },
      ],
    },
  ],
};
</script>
