<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "3e69364f-6e96-494a-96b3-6c82d3e8bed9",
  name: "Spina Astera",
  imageSrc: "/images/spina-astera.jpg",
  imageAlt: "Spina Astera",
  position: "object-center",
  derp: {
    imageSrc: "/images/spina-astera.jpg",
    imageAlt: "Derp Spina Astera",
    position: "object-center",
  }
};

const signets = {
  builds: [
    {
      name: "First Variation",
      recommended: "HoD",
      boss: "",
      supports: [
        {
          time: "Early",
          sigils: "Golden Goblet",
          support_1: "AE",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "Burden / Because of You",
          support_1: "AE",
          support_2: "LE / BR",
        },
        {
          time: "Late",
          sigils: "Home Lost / Dreamful Gold",
          support_1: "AE",
          support_2: "BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Wild Flare",
              desc: "Each hit of Astral Flare unleashes Astral Flare: Erupt, casting 1 Astral Rend in front that deals 200% of ATK as Fire DMG. Each cast of Astral Rend exits Astral Harness state, restoring 3 SP and 80 Astrum, with a maximum of 6 casts",
              priority: "Start",
            },
            {
              name: "Blessing of Radiant Formation",
              desc: "Hits dealt by Astral Flare: Erupt +1. After unleashing Astral Flare: Erupt, the remaining Ultimate CD reduces by 10% and 300 Astrum is restored",
              priority: "1st",
            },
            {
              name: "Blessing of Holy Flame",
              desc: "Astral Flare deals an additional 500% ATK of Fire DMG to the target for every 6 hits and increases the Fire DMG to the hit target by 20% (independent effect) for 5s. Can be refreshed",
              priority: "2nd",
            },
            {
              name: "Blessing of Star Quillon",
              desc: "When unleashing Astral Flare: Ignite, and Astral Flare: Combust, the 4th hit of Basic ATK in Astral Harness state deals 500% of ATK as Fire DMG to enemies within 10m, pulls them towards Valkyrie, and increases the total DMG taken by the target by 20%",
              priority: "Filler",
            },
            {
              name: "Blessing of Alrescha",
              desc: "Hits dealt by Astral Flare +1. When Astral Flare hits the target, its Fire DMG increases by 40% for 5s. This effect can be refreshed",
              priority: "Optional",
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
          name: "Pardofelis 1",
          lists: [
            {
              name: "Merchant's Philosophy",
              desc: "After finishing each floor, the number of currently owned Shiny Silvers grows by 10% for up to 100 (independent effect)",
              priority: "1st",
            },
            {
              name: "Shiny & Valuable",
              desc: "Enemy kills grant bonus Shiny Silvers. Non-boss enemies grant 5 each. Boss enemies grant 100 each (independent effect)",
              priority: "2nd",
            },
            {
              name: "Back-Curled Tail",
              desc: "Every 100 Shiny Silvers obtained this round boost Physical and Elemental MG by 0.8%",
              priority: "3rd",
            },
            {
              name: "Flexible P&C",
              desc: "Every 100 Shiny Silvers obtained this round restore 1 HP and 0.1 SP. Taking DMG disables this effect for 5s",
              priority: "Optional (Kalpas2 synergy)",
            },
            {
              name: "Nexus Signet: Empty Dreams, Self, Set, and Joy",
              desc: "Reaching 500 Shiny Silvers boosts the effects of all Normal Signets of Reverie by 25%. Reaching 1000 boosts the effects by 50% and Physical and Elemental DMG by 60%",
              priority: "CORE",
            },
            {
              name: "This Is Not Where We Die",
              desc: "Valkyries enters with a Good Luck shield. While the shield holds, every 100 Shiny Silvers owned grant 1% Physical and Elemental Breach. The shield can block incoming MG twice before it breaks, and every 500 Shiny Silvers owned grant one more block",
              priority: "Optional",
            },
          ],
        },
      ],
    },
    {
      name: "Second Variation",
      recommended: "HoD",
      boss: "",
      supports: [
        {
          time: "Early",
          sigils: "Golden Goblet",
          support_1: "AE",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "Burden / Because of You",
          support_1: "AE",
          support_2: "LE / BR",
        },
        {
          time: "Late",
          sigils: "Home Lost / Dreamful Gold",
          support_1: "AE",
          support_2: "BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Wild Flare",
              desc: "Each hit of Astral Flare unleashes Astral Flare: Erupt, casting 1 Astral Rend in front that deals 200% of ATK as Fire DMG. Each cast of Astral Rend exits Astral Harness state, restoring 3 SP and 80 Astrum, with a maximum of 6 casts",
              priority: "Start",
            },
            {
              name: "Blessing of Radiant Formation",
              desc: "Hits dealt by Astral Flare: Erupt +1. After unleashing Astral Flare: Erupt, the remaining Ultimate CD reduces by 10% and 300 Astrum is restored",
              priority: "1st",
            },
            {
              name: "Blessing of Holy Flame",
              desc: "Astral Flare deals an additional 500% ATK of Fire DMG to the target for every 6 hits and increases the Fire DMG to the hit target by 20% (independent effect) for 5s. Can be refreshed",
              priority: "2nd",
            },
            {
              name: "Blessing of Star Quillon",
              desc: "When unleashing Astral Flare: Ignite, and Astral Flare: Combust, the 4th hit of Basic ATK in Astral Harness state deals 500% of ATK as Fire DMG to enemies within 10m, pulls them towards Valkyrie, and increases the total DMG taken by the target by 20%",
              priority: "Filler",
            },
            {
              name: "Blessing of Alrescha",
              desc: "Hits dealt by Astral Flare +1. When Astral Flare hits the target, its Fire DMG increases by 40% for 5s. This effect can be refreshed",
              priority: "Optional",
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
          ],
        },
        {
          name: "Pardofelis (No Core)",
          lists: [
            {
              name: "Flexible P&C",
              desc: "Every 100 Shiny Silvers obtained this round restore 1 HP and 0.1 SP. Taking DMG disables this effect for 5s",
              priority: "YES",
            },
          ],
        },
      ],
    },
    {
      name: "Third Variation",
      recommended: "Choose HoD. Can swap \"Boundless Feeling\" to another Flamechaser's Support Skill if done take all recommended Aponia's Signets. For example, \"Falling in Past Light\" (especially if have \"Sneer\") to reduce Weapon active skill CD. Just make sure to guarantee gather with SpA. Ref: <a class='italic font-bold underline' href='https://www.youtube.com/watch?v=FIj1BNpKpLw'>here</a>",
      boss: "",
      supports: [
        {
          time: "Early",
          sigils: "Veil of Tears & Boundless Feeling",
          support_1: "AE",
          support_2: "BR",
        },
        {
          time: "Mid",
          sigils: "Veil of Tears & Boundless Feeling",
          support_1: "AE",
          support_2: "BR",
        },
        {
          time: "Late",
          sigils: "Veil of Tears & Boundless Feeling",
          support_1: "AE",
          support_2: "BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          info: "Double Ego Signet is a must",
          lists: [
            {
              name: "Blessing of Wild Flare",
              desc: "Each hit of Astral Flare unleashes Astral Flare: Erupt, casting 1 Astral Rend in front that deals 200% of ATK as Fire DMG. Each cast of Astral Rend exits Astral Harness state, restoring 3 SP and 80 Astrum, with a maximum of 6 casts",
              priority: "Start",
            },
            {
              name: "Blessing of Radiant Formation",
              desc: "Hits dealt by Astral Flare: Erupt +1. After unleashing Astral Flare: Erupt, the remaining Ultimate CD reduces by 10% and 300 Astrum is restored",
              priority: "Start",
            },
            {
              name: "Blessing of Holy Flame",
              desc: "Astral Flare deals an additional 500% ATK of Fire DMG to the target for every 6 hits and increases the Fire DMG to the hit target by 20% (independent effect) for 5s. Can be refreshed",
              priority: "1st",
            },
            {
              name: "Blessing of Star Quillon",
              desc: "When unleashing Astral Flare: Ignite, and Astral Flare: Combust, the 4th hit of Basic ATK in Astral Harness state deals 500% of ATK as Fire DMG to enemies within 10m, pulls them towards Valkyrie, and increases the total DMG taken by the target by 20%",
              priority: "Filler",
            },
            {
              name: "Blessing of Alrescha",
              desc: "Hits dealt by Astral Flare +1. When Astral Flare hits the target, its Fire DMG increases by 40% for 5s. This effect can be refreshed",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Aponia 2",
          lists: [
            {
              name: "First, No Betrayal",
              desc: "Exhortation increases by 5 per second and caps at 200. Basic ATK's Total DMG increases by 0.3% of Exhortation. Triggering Ultimate Evasion Skill reduces 50% Exhortation",
              priority: "1st",
            },
            {
              name: "Third, No Brutality",
              desc: "Exhortation increases by 5 per second and caps at 200. Valkyrie has bonus SP regen per second equal to 1% of Exhortation. Reaching 160 combo reduces 50% Exhortation",
              priority: "2nd",
            },
            {
              name: "Fifth, No Falsehood",
              desc: "Valkyrie starts with 70 bonus Exhortation. Whenever Exhortation is reduced, enemies take 25% bonus Total DMG for 5s. Can be refreshed",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: You Shall Receive Discipline's Blessing",
              desc: "Normal Signet of Discipline grants Exhortation 100% increase per second. When Exhortation exceeds 150, You Shall Know Your Sins will trigger every 5s around the Valkyrie, dealing 1400% ATK of Adaptive DMG. The Valkyrie deals 10% more Total DMG for each enemy hit, for a total of 70%, for 10s. Triggering it again resets the duration",
              priority: "CORE",
            },
            {
              name: "You Shall Punish Evil",
              desc: "You Shall Know Your Sins Total DMG dealt increases 45% and increases Physical and Elemental Breach by 0.25% of Exhortation for 6s upon hitting an enemy. Triggering it again resets the duration",
              priority: "YES",
            },
            {
              name: "You Shall Follow Good",
              desc: "You Shall Know Your Sins Total DMG dealt increases 45% and increases Physical and Elemental Breach by 0.25% of Exhortation for 6s upon hitting an enemy. Triggering it again resets the duration",
              priority: "1st",
            },
            {
              name: "You Shall Answer Prayers",
              desc: "Triggering You Shall Know Your Sins causes the Valkyrie to enter Penance for 8s. In Penance, the Valkyrie takes 30% less total DMG and deals 45% more Physical and Elemental DMG to enemies. Valkyrie deals 800% ATK of Adaptive DMG to attacking enemies when hit; CD: 5s. Triggering it again resets the duration",
              priority: "2nd",
            },
          ],
        },
        {
          name: "Eden 2",
          info: "Build this or Griseo based on RNG Luck. Build Griseo after this build complete. \"Withered Soil\" is not necessary but can paired with Elysia: \"Radiant Formation\"",
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
              priority: "Optional",
            },
            {
              name: "Echo of Withered Soil",
              desc: "After lasting over 7s in Final Note, boost SP cap and restore SP/s till it ends",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Griseo 2",
          info: "Build this or Eden based on RNG Luck. Build Eden After this build complete",
          lists: [
            {
              name: "Red & Hot",
              desc: "Using a weapon active taints enemies nearby with red paint for 8s and makes them take 25% bonus Physical and Elemental DMG (cannot stack). Triggering it again resets the duration",
              priority: "1st",
            },
            {
              name: "Yellow & Warm",
              desc: "Using an Ultimate taints enemies nearby with yellow paint for 8s and makes them take 30% bonus Total DMG. Triggering it again resets the duration",
              priority: "2nd",
            },
            {
              name: "Blue & Cold",
              desc: "Triggering an Ultimate Evasion Skill taints enemies nearby with blue paint for 8s and reduces their Total DMG and Move Speed by 30%. Triggering it again resets the duration",
              priority: "3rd",
            },
            {
              name: "Grey & Empty",
              desc: "Enemies stay tainted for 5s longer",
              priority: "Optional",
            },
            {
              name: "Nexus Signet: Faded Stars",
              desc: "When tainted enemies are tainted another color, Blending is triggered, dealing 300% ATK of Adaptive DMG to enemies within 15m and tainting enemies purple, green, or orange based on the Enhanced Signet; CD: 1s. Total DMG increases 15% for each layer of taint, plus an additional 15% for enemies of a countered type",
              priority: "CORE",
            },
            {
              name: "A Flame Extinguished",
              desc: "When red and yellow taint triggers Blending you become tainted orange for 15s, triggering Time Fracture for 2.5s and reducing enemy Physical Defense 40% and Elemental Resist 15% for 10s; CD: 7s. Triggering it again resets the duration",
              priority: "1st",
            },
            {
              name: "Petals In the Wind",
              desc: "When red and blue taint triggers Blending, enemies within 8m are dealt 1200%/500% ATK of Adaptive DMG; CD: 3s. Also taints yourself purple for 15s, increasing the effect of red, yellow, and blue taint by 40%. Triggering it again resets the duration",
              priority: "3rd",
            },
            {
              name: "Fallen Leaves",
              desc: "When yellow and blue taint triggers Blending along with an AoE ATK dealing 800% ATK of Adaptive DMG; CD: 3s. Also taints yourself green for 15s, increasing Total DMG 20% for each taint in Faded Stars. Triggering it again resets the duration",
              priority: "3rd",
            },
          ],
        },
        {
          name: "Kevin 1 (Choose one)",
          info: "Can take \"Goblet of the Pilgrim\" when Paired with Eden: \"Echo of Withered Soil\"",
          lists: [
            {
              name: "Goblet of the Giver",
              desc: "Ultimate boosts Total DMG by 35% for 5s",
              priority: "1st",
            },
            {
              name: "Brand of the Undead",
              desc: "Ultimate boosts Elemental DMG by 30% for 5s",
              priority: "2nd",
            },
            {
              name: "Artifact of the Inhibitor",
              desc: "Ultimate boosts Elemental Breach by 20% for 5s",
              priority: "3rd",
            },
            {
              name: "Artifact of the Inhibitor",
              desc: "Ultimate boosts Elemental Breach by 20% for 5s",
              priority: "3rd",
            },
            {
              name: "Rochet of the Pilgrim",
              desc: "Ultimate restores 3 SP per second for 5s",
              priority: "Optional",
            },
            {
              name: "Nexus Signet: Blade of the Deliverer",
              desc: "Ultimate triggers Final Battle status during which all buffs provided by Normal Signets of Deliverance increase by for 5s",
              priority: "CORE",
            },
          ],
        },
        {
          name: "Kalpas 2 (Choose one)",
          lists: [
            {
              name: "Bone, Blood, and Ribbon",
              desc: "Every 100 HP loss boosts Physical & Elemental DMG by 0.8%",
              priority: "1st",
            },
            {
              name: "Blade, Grave, and Scar",
              desc: "Every 100 HP loss boosts Total DMG by 1.0%",
              priority: "2nd",
            },
            {
              name: "Path, Misfortune, and Written Fate",
              desc: "Max HP increases by 25%",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Soldiers, Scissors, Spoils, and Slaughter",
              desc: "Valkyrie's current HP cannot exceed 18% of her Max HP, and if the HP recovery in combat reaches 0/400/800, the recovery amount increases by of the Bloodboil Armor charges, up to for a single charge. The charge cap is 1800, and each point increases the HP cap by 1",
              priority: "CORE",
            },
          ],
        },
        {
          name: "Su 2 (Choose one)",
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
          name: "Vill-V (No Core, Optional)",
          info: "Can Build this either from Shop or Bad RNG Luck",
          lists: [
            {
              name: "Act VI: Sneer",
              desc: "Using a weapon active restores 12 SP in 5s and reduces its CD by 15%",
              priority: "Filler",
            },
            {
              name: "Act II: Pendulum",
              desc: "Using a weapon active makes enemies take 20% bonus Total DMG for 3.5s. Triggering it again resets the duration",
              priority: "Filler",
            },
            {
              name: "Act IV: Spoon",
              desc: "Using a weapon active boosts Physical DMG and Elemental DMG from Charge ATK and Combo ATK by 25% for 3.5s Triggering it again resets the duration",
              priority: "Filler",
            }
          ],
        },
      ],
    },
  ],
};
</script>