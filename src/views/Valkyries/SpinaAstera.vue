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
  position: "object-top",
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
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "",
          support_2: "",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "",
          support_2: "",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "",
          support_2: "",
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
              priority: "Filler",
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
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "",
          support_2: "",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "",
          support_2: "",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "",
          support_2: "",
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
              priority: "Filler",
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
  ],
};
</script>