<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "51dcbcbd-8bfd-4916-8801-aee9f9cfe186",
  name: "Argent Knight: Artemis",
  imageSrc: "/images/argent-knight-artemis.jpg",
  imageAlt: "Argent Knight: Artemis",
  position: "object-center",
};

const signets = {
  builds: [
    {
      name: "Recommendation",
      supports: [
        {
          time: "Early",
          sigils: "Forbidden Seed / Burden",
          support_1: "AE",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "Golden Goblet / Light as a Leaf",
          support_1: "AE",
          support_2: "LE / HB",
        },
        {
          time: "Late",
          sigils: "Home Lost",
          support_1: "AE",
          support_2: "HB",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Winter Harvest",
              desc: "Enemies recovering from Ice Cell are inflicted with 1 stack of Hypothermia",
              priority: "Start",
            },
            {
              name: "Blessing of Stellar Trials",
              desc: "Inflicting Ice Cell also creates a Frost Ring centered around the target lasting 2s which deals 480% ATK of Ice DMG per 0.3s to enemies nearby",
              priority: "1st",
            },
            {
              name: "Blessing of Frost Scythe",
              desc: "Tap [ATK] after evasion to hurl Frost Guisarmier which spins for 5s, gathers enemies nearby, and deal 5400% ATK of Ice DMG. CD: 10s",
              priority: "2nd",
            },
            {
              name: "Blessing of Cold Moon",
              desc: "Inflicting Ice Cell also creates a self-centered Frost Ring lasting 6s which deals 180% ATK of Ice DMG per 0.3s to enemies nearby",
              priority: "Optional",
            },
            {
              name: "Blessing of Uranian Mirror",
              desc: "Burst mode consumes 100% more SP and Valkyrie deals 90% bonus Total DMG in burst mode",
              priority: "Filler",
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
          name: "Kevin 2",
          lists: [
            {
              name: "Rochet of the Pilgrim",
              desc: "Ultimate restores 3 sp per second for 5s",
              priority: "YES",
            },
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
              desc: "Ultimate or burst mode ATKs hitting enemies 50 times triggers War of Deliverance status during which all buffs provided by Normal Signets of Deliverance are active",
              priority: "CORE",
            },
            {
              name: "Dream of the Deliverer",
              desc: "While War of the Deliverer is active increase normal signets of Deliverance effects by 50%",
              priority: "YES",
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
              desc: "Bodhi Open Eye debuffs last 3 seconds longer and every debuff on the enemy boosts Total DMG taken by 5%",
              priority: "Optional",
            },
          ],
        },
      ],
    },
  ],
};
</script>