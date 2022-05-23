<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "58e4c48d-a200-4663-b184-e0c39c7a2a55",
  name: "Miss Pink Elf",
  imageSrc: "/images/miss-pink-elf.png",
  imageAlt: "Miss Pink Elf",
  position: "object-left",
  derp: {
    imageSrc: "/images/derp/miss-pink-elf.png",
    imageAlt: "Derp Miss Pink Elf",
    position: "object-center",
  }
};

const signets = {
  builds: [
    {
      name: "First Variation",
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "VC",
          support_2: "DP",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "VC",
          support_2: "DP / SS",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "VC",
          support_2: "SS",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Purity",
              desc: "While Ultimate is active, a wave of ricochet occurs under Flawless Dome every second. The ricochets triggered in this way only ricochet 3 times but deal 130% ATK of Physical DMG. (DMG Source: Ultimate)",
              priority: "Start",
            },
            {
              name: "Blessing of Zenith",
              desc: "While Ultimate is active, each ricochet deals 15% ATK of bonus Physical DMG on hit. Every wave of ricochet reduces weapon active's CD by 0.6s",
              priority: "Start",
            },
            {
              name: "Blessing of Love",
              desc: "While Ultimate is active, Charged Shot: Cupid's Bolt consumes 100% bonus Infatuation and deals 700% ATK of bonus Physical DMG",
              priority: "1st",
            },
            {
              name: "Blessing of Benevolence",
              desc: "Infatuation is fully restored when Ultimate Evasion Skill is triggered. If Infatuation drops below 100 after using Charged Shot: Cupid's Bolt, you can consume 1 Ultimate Evasion charge to trigger Ultimate Evasion Skill",
              priority: "Filler",
            },
            {
              name: "Blessing of Beauty",
              desc: "Using weapon active restores 1 additional Ultimate Evasion charge. Enemies take 25% bonus Total DMG when a Crystalline Seed is attached to them",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Kevin 2",
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
              desc: "Ultimate or burst mode ATKs hitting enemies 50 times triggers War of Deliverance status during which all buffs provided by Normal Signets of Deliverance are active",
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
              name: "Recitatif of Fine Jade",
              desc: "Initial SP and max SP increase by 30",
              priority: "2nd",
            },
            {
              name: "Recitatif of Birds",
              desc: "Every 10 SP left reduces Total DMG taken by 2.5%",
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
            {
              name: "Dictum of Anatman",
              desc: "The Bodhi: Eyes Open lasts for 3s longer. For every debuff on the target enemy, it takes 5% bonus Total DMG",
              priority: "Optional",
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
    {
      name: "Second Variation",
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "VC",
          support_2: "DP",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "VC",
          support_2: "DP / SS",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "VC",
          support_2: "SS",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Purity",
              desc: "While Ultimate is active, a wave of ricochet occurs under Flawless Dome every second. The ricochets triggered in this way only ricochet 3 times but deal 130% ATK of Physical DMG. (DMG Source: Ultimate)",
              priority: "Start",
            },
            {
              name: "Blessing of Zenith",
              desc: "While Ultimate is active, each ricochet deals 15% ATK of bonus Physical DMG on hit. Every wave of ricochet reduces weapon active's CD by 0.6s",
              priority: "Start",
            },
            {
              name: "Blessing of Love",
              desc: "While Ultimate is active, Charged Shot: Cupid's Bolt consumes 100% bonus Infatuation and deals 700% ATK of bonus Physical DMG",
              priority: "1st",
            },
            {
              name: "Blessing of Benevolence",
              desc: "Infatuation is fully restored when Ultimate Evasion Skill is triggered. If Infatuation drops below 100 after using Charged Shot: Cupid's Bolt, you can consume 1 Ultimate Evasion charge to trigger Ultimate Evasion Skill",
              priority: "Filler",
            },
            {
              name: "Blessing of Beauty",
              desc: "Using weapon active restores 1 additional Ultimate Evasion charge. Enemies take 25% bonus Total DMG when a Crystalline Seed is attached to them",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Kevin 2",
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
              desc: "Ultimate or burst mode ATKs hitting enemies 50 times triggers War of Deliverance status during which all buffs provided by Normal Signets of Deliverance are active",
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
              name: "Recitatif of Fine Jade",
              desc: "Initial SP and max SP increase by 30",
              priority: "2nd",
            },
            {
              name: "Recitatif of Birds",
              desc: "Every 10 SP left reduces Total DMG taken by 2.5%",
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
              priority: "YES",
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
              desc: "Valkyrie's current HP cannot exceed 18% of her Max HP, and if the HP recovery in combat reaches 0/400/800, the recovery amount increases by of the Bloodboil Armor charges, up to for a single charge. The charge cap is 1800, and each point increases the HP cap by 1",
              priority: "CORE",
            },
            {
              name: "Death, Life, Oblivion, and Existence",
              desc: "The Bloodboil Armor charges cap increases by 500. At over 1500 charges, Bloodboil Armor can absorb DMG equal to 1% of its charges",
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