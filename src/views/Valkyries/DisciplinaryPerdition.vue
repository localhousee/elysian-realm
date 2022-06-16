<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "3d4d0ed7-e673-4d74-90fd-8143ce884e55",
  name: "Disciplinary Perdition",
  imageSrc: "/images/disciplinary-perdition.jpg",
  imageAlt: "Disciplinary Perdition",
  position: "object-top",
  derp: {
    imageSrc: "/images/derp/disciplinary-perdition.png",
    imageAlt: "Derp Disciplinary Perdition",
    position: "object-center",
  }
};

const signets = {
  builds: [
    {
      name: "Auto Attack Spam",
      recommended: "Husk",
      boss: "",
      supports: [
        {
          time: "Early",
          sigils: "Veil of Tears / Hometown",
          support_1: "AE",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "Rainbow of Absence / The Lonely Moon",
          support_1: "AE",
          support_2: "LE / BR",
        },
        {
          time: "Late",
          sigils: "Resolve / Hometown",
          support_1: "AE",
          support_2: "BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Shelter",
              desc: "In Predictor's Sentence form, Redemption cost per second reduced by 55%; Total DMG dealt by Thunderstorm and Inhibitor's Adjudication increases 70% and count as Ultimates",
              priority: "Start",
            },
            {
              name: "Blessing of Inclusiveness",
              desc: "Restores 12 SP and reduces Ultimate CD by 6s when illusion uses QTE. Increases Ultimate's Total DMG by 60%. Ultimate restores up to 100% Redemption when used",
              priority: "Start",
            },
            {
              name: "Blessing of Admonition",
              desc: "Aponia gains 40% Total DMG Reduction. In Predictor's Sentence form, Lightning DMG increases 30% every 0.5s for a maximum of 180%. Inhibitor's Adjudication deals an additional 400% Lightning DMG",
              priority: "1st",
            },
            {
              name: "Blessing of Atonement",
              desc: "Aponia illusory Summoned Entity wherever she does, dealing 385% Lightning DMG every second to surrounding enemies. The illusion's Total DMG increases 100% and restores 12 SP after leaving Predictor's Sentence form",
              priority: "2nd",
            },
            {
              name: "Blessing of Rescue",
              desc: "Illusory Summoned Entity will deal Paralyse Trauma alongside DMG. DMG dealt by your Ultimate Evasion Skill increases 120%. Lightning DMG dealt by you or your illusion increases 70%",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Aponia 1",
          lists: [
            {
              name: "Fourth, No Insolence",
              desc: "Exhortation increases by 5 per second and caps at 200. Ultimate's Physical and Elemental DMG increases by 0.3% of of Exhortation. Using weapon skills reduces 50% Exhortation",
              priority: "1st",
            },
            {
              name: "Fifth, No Falsehood",
              desc: "Valkyrie starts with 70 bonus Exhortation. Whenever Exhortation is reduced, enemies take 25% bonus Total DMG for 5s. Can be refreshed",
              priority: "2nd",
            },
            {
              name: "First, No Betrayal",
              desc: "Exhortation increases by 5 per second and caps at 200. Basic ATK's Total DMG increases by 0.3% of Exhortation. Triggering Ultimate Evasion Skill reduces 50% Exhortation",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: You Shall Be Subject to Numerous Disciplines",
              desc: "Reaching 120 Exhortation induces Mortification where Valkyrie Total DMG increases by 25% of Exhortation. Also, for every Signet of Discipline unlocked, Valkyrie deals 5% bonus Physical DMG and Elemental DMG",
              priority: "CORE",
            },
            {
              name: "You Shall Be Bound by Thy Body",
              desc: "In Mortification, Basic ATK has 30% Physical Breach and Elemental Breach but Ultimate deals 20% less Total DMG",
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
      ],
    },
    {
      name: "Ultimate & Golden Spam",
      recommended: "Husk",
      boss: "",
      supports: [
        {
          time: "Early",
          sigils: "Burden / Hometown",
          support_1: "AE",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "Rainbow of Absence / The Lonely Moon",
          support_1: "AE",
          support_2: "LE / BR",
        },
        {
          time: "Late",
          sigils: "Resolve / Hometown",
          support_1: "AE",
          support_2: "BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Shelter",
              desc: "In Predictor's Sentence form, Redemption cost per second reduced by 55%; Total DMG dealt by Thunderstorm and Inhibitor's Adjudication increases 70% and count as Ultimates",
              priority: "Start",
            },
            {
              name: "Blessing of Inclusiveness",
              desc: "Restores 12 SP and reduces Ultimate CD by 6s when illusion uses QTE. Increases Ultimate's Total DMG by 60%. Ultimate restores up to 100% Redemption when used",
              priority: "Start",
            },
            {
              name: "Blessing of Admonition",
              desc: "Aponia gains 40% Total DMG Reduction. In Predictor's Sentence form, Lightning DMG increases 30% every 0.5s for a maximum of 180%. Inhibitor's Adjudication deals an additional 400% Lightning DMG",
              priority: "1st",
            },
            {
              name: "Blessing of Atonement",
              desc: "Aponia illusory Summoned Entity wherever she does, dealing 385% Lightning DMG every second to surrounding enemies. The illusion's Total DMG increases 100% and restores 12 SP after leaving Predictor's Sentence form",
              priority: "2nd",
            },
            {
              name: "Blessing of Rescue",
              desc: "Illusory Summoned Entity will deal Paralyse Trauma alongside DMG. DMG dealt by your Ultimate Evasion Skill increases 120%. Lightning DMG dealt by you or your illusion increases 70%",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Kevin 1",
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
              desc: "Every 10 SP left reduces Total DMG taken by 2.5%",
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
              desc: "After lasting over 7s, reduce ATK, DEF, ele resists of enemies nearby",
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
