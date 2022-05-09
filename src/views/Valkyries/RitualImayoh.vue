<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "50289333-4dd5-46b8-a315-d357e4eabb78",
  name: "Ritual Imayoh",
  imageSrc: "/images/ritual-imayoh.jpg",
  imageAlt: "Ritual Imayoh",
  position: "object-right-top",
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
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "VC",
          support_2: "LE / BR",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "VC",
          support_2: "BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Prosperity",
              desc: "Tap [ATK] after evasion to dash to enemies for an aerial kick, which can be connected into Basic ATK Sequence 4. Basic ATK Sequence 6 restores KE every time it lands",
              priority: "Start",
            },
            {
              name: "Blessing of Dawn",
              desc: "At full KE, the next Combo ATK consumes all of it to constitute 4 stacks and additionally fire 4 homing missiles dealing 3600% ATK of Physical DMG",
              priority: "1st",
            },
            {
              name: "Blessing of Blossom",
              desc: "Homing missiles restore 2 SP on hit. Basic ATK Sequence 6 additionally fires 4 homing missiles each dealing 200% ATK of Physical DMG",
              priority: "2nd",
            },
            {
              name: "Blessing of Fertility",
              desc: "Ultimate replenishes 40 light bullets for every gun turret and boosts their Tech Level by 1 (caps at 3). Each turret restores Tech Level x 30 KE per second",
              priority: "No",
            },
            {
              name: "Blessing of Torch",
              desc: "When a Combo ATK with KE consumed hits, all gun turrets fire a laser beam at the target to deal Combo ATK stacks x 1600% ATK of Physical DMG",
              priority: "No",
            },
          ],
        },
        {
          name: "Mobius 1",
          lists: [
            {
              name: "Lip Poison [E]",
              desc: "Total DMG from summoned entities, ELFs, and Support Valkyries increases by 60%. ELFs",
              priority: "1st",
            },
            {
              name: "Lodging [C]",
              desc: "ELF Ultimates and Support Valkyries support skills have 20% reduced CD",
              priority: "2nd",
            },
            {
              name: "Entwined [P]",
              desc: "For every summoned entity, ELF, or Support Valkyrie present, enemies take 8% bonus Total DMG (5 stacks max)",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Infinite [X]",
              desc: "Summoning summoned entities or using ELF Ultimates triggers Mind Sync state which lasts 8s. In Mind Sync, Valkyrie herself, summoned entities, ELFs, and Support Valkyries deal 30% bonus Physical and Elemental DMG. Reset on exiting Mind Sync",
              priority: "CORE",
            },
            {
              name: "Dead [X]",
              desc: "For every second in Mind Sync, Valkyrie herself, summoned entities, ELFs, and Support Valkyries deal 10% bonus Total DMG. 5 stacks max. 9 stacks max with any summoned entity present. Reset on exiting Mind Sync",
              priority: "YES",
            },
            {
              name: "Newborn [X]",
              desc: "Triggering Mind Sync again during Mind Sync no longer resets the duration but extends the duration by 4.0s instead. With any summoned entity present, the duration is extended by 5s additionally",
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
      ],
    },
  ],
};
</script>