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
    imageSrc: "/images/disciplinary-perdition.jpg",
    imageAlt: "Derp Disciplinary Perdition",
    position: "object-center",
  }
};

const signets = {
  builds: [
    {
      name: "Auto Attack Spam",
      supports: [
        {
          time: "Early",
          sigils: "Memory / Hometown",
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
              name: "Blessing of Adtontament",
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
            {
              name: "Dictum of Anatman",
              desc: "Bodhi Open Eye debuffs last 3 seconds longer and every debuff on the enemy boosts Total DMG taken by 5%",
              priority: "Optional",
            },
          ],
        },
      ],
    },
    {
      name: "Stars (Griseo)",
      supports: [
        {
          time: "Early",
          sigils: "Memory / Hometown",
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
                name: "Blessing of Admonition",
                desc: "Aponia gains 40% Total DMG Reduction. In Predictor's Sentence form, Lightning DMG increases 30% every 0.5s for a maximum of 180%. Inhibitor's Adjudication deals an additional 400% Lightning DMG",
                priority: "Start",
              },
            {
              name: "Blessing of Inclusiveness",
              desc: "Restores 12 SP and reduces Ultimate CD by 6s when illusion uses QTE. Increases Ultimate's Total DMG by 60%. Ultimate restores up to 100% Redemption when used",
              priority: "1st",
            },
            {
              name: "Blessing of Adtontament",
              desc: "Aponia illusory Summoned Entity wherever she does, dealing 385% Lightning DMG every second to surrounding enemies. The illusion's Total DMG increases 100% and restores 12 SP after leaving Predictor's Sentence form",
              priority: "Filler",
            },
            {
              name: "Blessing of Rescue",
              desc: "Illusory Summoned Entity will deal Paralyse Trauma alongside DMG. DMG dealt by your Ultimate Evasion Skill increases 120%. Lightning DMG dealt by you or your illusion increases 70%",
              priority: "Filler",
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
                name: "Blue & Cold",
                desc: "Triggering an Ultimate Evasion Skill taints enemies nearby with blue paint for 8s and reduces their Total DMG and Move Speed by 30%. Triggering it again resets the duration",
                priority: "3rd",
              },
            {
              name: "Grey & Empty",
              desc: "Enemies stay tainted for 5s longer",
              priority: "4th",
            },
            {
              name: "Nexus Signet: Shine like Stars",
              desc: "When there are enemies tainted with 1/2/3 different paints, Valkyries deal 20%/50%/100% bonus Total DMG to enemies of countering types",
              priority: "CORE",
            },
            {
              name: "Burning Like Flames",
              desc: "When enemies are tainted with both yellow and red paints, Valkyries have 25% bonus Physical and Elemental Breach against them",
              priority: "1st",
            },
            {
              name: "Blooming like Flowers",
              desc: "When enemies of countering types are tainted with both blue and red paints, Valkyries deal 50% bonus Total DMG to them (cannot stack)",
              priority: "2nd",
            },
            {
              name: "Stretching Like Leaves",
              desc: "When enemies are tainted with both yellow and blue paints, Valkyrie attacks against them deal 3000% ATK of bonus Adaptive DMG to enemies within 6 meters. CD: 8s",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Kevin 2",
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
              name: "Rochet of Pilgrim",
              desc: "Ultimate restores 3 SP per second for 5s",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Shadow of the Deliverer",
              desc: "Ultimate or burst mode ATKs hitting enemies 50 times triggers War of Deliverance status during which all buffs provided by Normal Signets of Deliverance are active",
              priority: "CORE",
            },
            {
              name: "Dream of the Deliverer",
              desc: "In War of Deliverance, all buffs provided by Normal Signets of Deliverance are enhanced by 50%",
              priority: "1st",
            },
            {
              name: "Triumph of the Deliverer",
              desc: "Entering War of Deliverance makes Valkyrie attacks ignore enemy DEF and Elemental Resists for 6s, after which all enemies take 20% bonus Total DMG",
              priority: "2nd",
            },
          ],
        },
      ],
    },
    {
      name: "Gold (Eden)",
      supports: [
        {
          time: "Early",
          sigils: "Memory / Hometown",
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
                name: "Blessing of Admonition",
                desc: "Aponia gains 40% Total DMG Reduction. In Predictor's Sentence form, Lightning DMG increases 30% every 0.5s for a maximum of 180%. Inhibitor's Adjudication deals an additional 400% Lightning DMG",
                priority: "Start",
              },
            {
              name: "Blessing of Inclusiveness",
              desc: "Restores 12 SP and reduces Ultimate CD by 6s when illusion uses QTE. Increases Ultimate's Total DMG by 60%. Ultimate restores up to 100% Redemption when used",
              priority: "1st",
            },
            {
              name: "Blessing of Adtontament",
              desc: "Aponia illusory Summoned Entity wherever she does, dealing 385% Lightning DMG every second to surrounding enemies. The illusion's Total DMG increases 100% and restores 12 SP after leaving Predictor's Sentence form",
              priority: "Filler",
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
              name: "Rochet of Pilgrim",
              desc: "Ultimate restores 3 SP per second for 5s",
              priority: "3rd",
            },
            {
              name: "Goblet of Giver",
              desc: "Ultimate boosts Total DMG by 35% for 5s",
              priority: "4th",
            },
            {
              name: "Nexus Signet: Shadow of the Deliverer",
              desc: "Ultimate or burst mode ATKs hitting enemies 50 times triggers War of Deliverance status during which all buffs provided by Normal Signets of Deliverance are active",
              priority: "CORE",
            },
            {
              name: "Dream of the Deliverer",
              desc: "In War of Deliverance, all buffs provided by Normal Signets of Deliverance are enhanced by 50%",
              priority: "1st",
            },
            {
              name: "Triumph of the Deliverer",
              desc: "Entering War of Deliverance makes Valkyrie attacks ignore enemy DEF and Elemental Resists for 6s, after which all enemies take 20% bonus Total DMG",
              priority: "2nd",
            },
          ],
        },
      ],
    },
  ],
};
</script>