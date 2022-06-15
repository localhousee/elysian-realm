<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "ec41c754-3ba9-4b03-8ad6-c9555838998e",
  name: "Infinite Ouroboros",
  imageSrc: "/images/infinite-ouroboros.jpg",
  imageAlt: "Infinite Ouroboros",
  position: "object-top",
  derp: {
    imageSrc: "/images/derp/infinite-ouroboros.png",
    imageAlt: "Derp Infinite Ouroboros",
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
          support_1: "AE",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "AE",
          support_2: "LE / BR",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "AE",
          support_2: "BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Ascension",
              desc: "When Umbra of Ouroboros is active, enemies are struck by lightning once per second and take 600% ATK of Lightning DMG (DMG source: Basic ATK)",
              priority: "Start",
            },
            {
              name: "Blessing of Ill Fortune",
              desc: "Ultimate deals 240% bonus Lightning DMG. Every Genesis Seed consumed reduces Ultimate CD by 0.5s",
              priority: "Start",
            },
            {
              name: "Blessing of Dark Assault",
              desc: "Basic/Charged/Combo ATKs deal 40% bonus Lightning DMG. Linked enemies hit by Basic/Charged/Combo ATKs pass on 12% of the DMG to other linked enemies",
              priority: "1st",
            },
            {
              name: "Blessing of Ravenousness",
              desc: "Exiting submerged mode deals 1600% ATK of AOE Lightning DMG and enemies hit take 30% bonus Combo ATK DMG in the next 5s (independent effect)",
              priority: "2nd",
            },
            {
              name: "Blessing of Mirage",
              desc: "In submerged mode, enemies in contact take 200% ATK of Lightning DMG per and take 35% bonus Total DMG for 8s",
              priority: "No",
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
              name: "Rochet of the Pilgrim",
              desc: "Ultimate restores 3 SP per second for 5s",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Blade of the Deliverer",
              desc: "Ultimate triggers Final Battle status during which all buffs provided by Normal Signets of Deliverance increase by for 5s",
              priority: "CORE",
            },
            {
              name: "Crusade of the Deliverer",
              desc: "After 3s into Final Battle, all buffs provided by Normal Signets of Deliverance increase by 90% instead of 50%",
              priority: "YES",
            },
            {
              name: "Echo of the Deliverer",
              desc: "Duration of Final Battle and all buffs provided by Normal Signets of Deliverance are extended to 8s",
              priority: "1st",
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
              priority: "2nd",
            },
          ],
        },
        {
          name: "Mobius 1",
          lists: [
            {
              name: "Lip Poison [E]",
              desc: "Total DMG from summoned entities, ELFs, and Support Valkyries increases by 60%",
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
          name: "Sakura 2 (Optional, one or none)",
          lists: [
            {
              name: "Bountiful Blossom: Ume",
              desc: "Triggering Ultimate Evasion Skill boosts Attack Speed & Move Speed by 40% for 8s",
              priority: "1st",
            },
            {
              name: "Bountiful Blossom: Koyo",
              desc: "Triggering Ultimate Evasion Skill boosts Total DMG taken by all enemies by 30% for 8s",
              priority: "2nd",
            },
            {
              name: "Bountiful Blossom: Fuji",
              desc: "Ultimate Evasion Skill has 1 more charge and 10% reduced CD",
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
          name: "Griseo 1 (Optional, one or none)",
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
              desc: "When there are enemies tainted with 1/2/3 different paints, Valkyries deal 20%/50%/100% bonus Total DMG to enemies of countering types",
              priority: "CORE",
            },
            {
              name: "Blooming like Flowers",
              desc: "When enemies of countering types are tainted with both blue and red paints, Valkyries deal 50% bonus Total DMG to them (cannot stack)",
              priority: "YES",
            },
          ],
        },
      ],
    },
  ],
}; 
</script>
