<template>
	<Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "7c932010-48c1-4ffe-8486-70fbb2347e93",
  name: "Luna Kindred",
  imageSrc: "/images/luna-kindred.jpg",
  imageAlt: "Luna Kindred",
  position: "object-center",
  derp: {
    imageSrc: "/images/luna-kindred.jpg",
    imageAlt: "Derp Luna Kindred",
    position: "object-center",
  }
};

const signets = {
  builds: [
    {
      name: "Recommendation",
      recommended: "Husk",
      boss: "",
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
          support_2: "LE / DP / BR",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "SS",
          support_2: "DP / BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Penumbra",
              desc: "Each Charged ATK only deals 140% ATK of Physical DMG, but every 4 consecutive Charged ATKs boost the speed of wielding the giant ax. Valkyrie gains a barrier with HP equal to 100% of her Max HP; when Sanguine Mark is below 50, every 3% Valkyrie HP will be converted to 1% barrier HP instead of Sanguine Mark cost",
              priority: "Start",
            },
            {
              name: "Blessing of Blood Feast",
              desc: "Within the next 8s after Ultimate's final hit lands, each Charged ATK deals bonus Physical DMG equal to 1.5x the amount of current HP loss",
              priority: "1st",
            },
            {
              name: "Blessing of Imprint",
              desc: "Every 2 Charged ATKs that consume Sanguine Mark will enable the next Charged ATK that consumes Sanguine Mark to deal bonus Physical DMG equal to 0.5x the amount of current HP loss",
              priority: "2nd",
            },
            {
              name: "Blessing of Immortality",
              desc: "Triggered once at below 1% HP to deal Physical DMG equal to 1.5x the amount of current HP loss to surrounding enemies every 0.8s for 4s, during which Valkyrie will not die and restores 5% HP afterward. This effect's triggering chance will be reset after Valkyrie HP rises back to 33%",
              priority: "No",
            },
            {
              name: "Blessing of Thirst",
              desc: "Lower HP enables higher HP recovery (max boost: 300%). If Valkyrie restores more than 10% HP within a short period of time, all enemies will be impaired for 10s (DEF -30%)",
              priority: "No",
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
              desc: "Hitting an enemy with 10 or more stacks of Rend triggers Evil's Doom which deals ATK of Adaptive 1500% DMG and 5000% ATK of bonus Adaptive DMG against shields. CD: 5s",
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