<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "b4d82c19-1ba8-4c31-9ff8-4697aba777d4",
  name: "Herrscher Of Sentience",
  imageSrc: "/images/herrscher-of-sentience.jpg",
  imageAlt: "Herrscher Of Sentience",
  position: "object-top",
};

const signets = {
  builds: [
    {
      name: "Stars (Griseo)",
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "BR",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "BR",
          support_2: "LE / SS",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "BR",
          support_2: "SS",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of  Victory",
              desc: "In Herrscher Form, Combo ATK: Slashes can have up to 18 slashes. After reaching 7 slashes, every slash deals 600% ATK of Physical DMG.",
              priority: "Start",
            },
            {
              name: "Blessing of Dark Plumes",
              desc: "Combo ATK restores 1 SP on hit and unleashes a plume attack on hit that deals 150% ATK of Physical DMG. CD: 0.5s",
              priority: "1st",
            },
            {
              name: "Blessing of Supremacy",
              desc: "Shield: I'm Untouchable absorbs 100% of DMG taken and deals 5000% ATK of Physical DMG to enemies within 8 metres when it ends or resets.",
              priority: "2nd",
            },
            {
              name: "Blessing of Legion",
              desc: "Sword, spear and chain combo attacks restore 300 sword, spear and chain energy respectively and boost Total DMG by 60% for 8s.",
              priority: "Filler",
            },
            {
              name: "Blessing of Ego",
              desc: "Casting Combo ATK summons an illusion (summoned entity) to replicate the attack. In Herrscher Form, the illusion only replicates the slashes each dealing 105% ATK of Physical DMG. The illusion has 400% of the Valkyrie's ATK.",
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
          name: "Kevin 1 (Choose one)",
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
          name: "Kevin 2 (Choose one)",
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
              name: "Nexus Signet: Shadow of the Deliverer",
              desc: "",
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
              desc: "",
              priority: "CORE",
            },
          ],
        },
      ],
    },
    {
      name: "Ego (Summoned Entities)",
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "BR",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "BR",
          support_2: "LE / SS",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "BR",
          support_2: "SS",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of  Victory",
              desc: "In Herrscher Form, Combo ATK: Slashes can have up to 18 slashes. After reaching 7 slashes, every slash deals 600% ATK of Physical DMG.",
              priority: "Start",
            },
            {
              name: "Blessing of Ego",
              desc: "Casting Combo ATK summons an illusion (summoned entity) to replicate the attack. In Herrscher Form, the illusion only replicates the slashes each dealing 105% ATK of Physical DMG. The illusion has 400% of the Valkyrie's ATK.",
              priority: "1st",
            },
            {
              name: "Blessing of Dark Plumes",
              desc: "Combo ATK restores 1 SP on hit and unleashes a plume attack on hit that deals 150% ATK of Physical DMG. CD: 0.5s",
              priority: "2nd",
            },
            {
              name: "Blessing of Supremacy",
              desc: "Shield: I'm Untouchable absorbs 100% of DMG taken and deals 5000% ATK of Physical DMG to enemies within 8 metres when it ends or resets.",
              priority: "3rd",
            },
            {
              name: "Blessing of Legion",
              desc: "Sword, spear and chain combo attacks restore 300 sword, spear and chain energy respectively and boost Total DMG by 60% for 8s.",
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
              desc: "",
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
              priority: "YES",
            },
          ],
        },
        {
          name: "Kevin 1 (Choose one)",
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
          name: "Kevin 2 (Choose one)",
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
      ],
    },
    {
      name: "Daybreak (Kosma)",
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "BR",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "BR",
          support_2: "LE / SS",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "BR",
          support_2: "SS",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of  Victory",
              desc: "In Herrscher Form, Combo ATK: Slashes can have up to 18 slashes. After reaching 7 slashes, every slash deals 600% ATK of Physical DMG.",
              priority: "Start",
            },
            {
              name: "Blessing of Dark Plumes",
              desc: "Combo ATK restores 1 SP on hit and unleashes a plume attack on hit that deals 150% ATK of Physical DMG. CD: 0.5s",
              priority: "1st",
            },
            {
              name: "Blessing of Supremacy",
              desc: "Shield: I'm Untouchable absorbs 100% of DMG taken and deals 5000% ATK of Physical DMG to enemies within 8 metres when it ends or resets.",
              priority: "2nd",
            },
            {
              name: "Blessing of Legion",
              desc: "Sword, spear and chain combo attacks restore 300 sword, spear and chain energy respectively and boost Total DMG by 60% for 8s.",
              priority: "Filler",
            },
            {
              name: "Blessing of Ego",
              desc: "Casting Combo ATK summons an illusion (summoned entity) to replicate the attack. In Herrscher Form, the illusion only replicates the slashes each dealing 105% ATK of Physical DMG. The illusion has 400% of the Valkyrie's ATK.",
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
              name: "Eyes that Overlook the Vicious Abyss",
              desc: "Each stack of Rend on enemies makes Valkyries deal 10% bonus DMG to their shields",
              priority: "Filler",
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
          name: "Kevin 1 (Choose one)",
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
          name: "Kevin 2 (Choose one)",
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
      ],
    },
  ],
};
</script>