<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "193a77a8-020d-4f1f-b47c-f602694efee6",
  name: "Golden Diva",
  imageSrc: "/images/golden-diva.jpg",
  imageAlt: "Golden Diva",
  position: "object-center",
  derp: {
    imageSrc: "/images/golden-diva.jpg",
    imageAlt: "Derp Argent Knight: Artemis",
    position: "object-center",
  }
};

const signets = {
  builds: [
    {
      name: "Combo Spam (No Ultimate)",
      supports: [
        {
          time: "Early",
          sigils: "Memory / Hometown",
          support_1: "AE",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "Light as a Bodhi Leaf / Because of You (5F)",
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
              name: "Blessing of Arioso",
              desc: "During Sound of Nature, each note consumed increases Total DMG by 12% with a max stack of 10. This is reset when Sound of Nature ends",
              priority: "Start",
            },
            {
              name: "Blessing of Fugue",
              desc: "Ensemble combo sequence is increased by 6. Hurling pistols Total DMG increases 140%",
              priority: "Start",
            },
            {
              name: "Blessing of Concerto",
              desc: "Each Combo ATK grants 1 Charge. At 4 Charge, Basic and Combo ATKs' Total DMG increase by 60% for 15s. Charge consumed on use and cannot be restored during use. Restores 12 SP after use",
              priority: "1st",
            },
            {
              name: "Blessing of Cadenza",
              desc: "Chord and Variation launch sound waves dealing 550% Lightning DMG. Each wave increases Total DMG reduction by 30% and slightly raises Ignore Interrupt for 10s while restoring 2 or 4 SP respectively. Triggering it again resets the duration",
              priority: "Filler",
            },
            {
              name: "Blessing of Symphony",
              desc: "Hurl pistols when using Ensemble Playing for 12 SP and dealing 350% Lightning DMG",
              priority: "No",
            },
          ],
        },
        {
          name: "Eden 1",
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
              name: "Nexus Signet: Aria of Gold",
              desc: "Restoring 100 SP in total triggers 3 Lightning of Aria bolts each dealing 450% ATK of Lightning DMG and inflicting 6s of Intoxicate randomly. Intoxicated enemies take 15% bonus Total DMG",
              priority: "CORE",
            },
            {
              name: "Aria of Soil",
              desc: "Intoxicated enemies take only 10% bonus Total DMG but it can stack up to 3 times",
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
              name: "Hometown, Homeland, Friends, and Acquaintances",
              desc: "If [Bloodboil Garment] exceeds 1500, gain 25% physical and elemental breach",
              priority: "YES",
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
          name: "Griseo 1 (Optional)",
          lists: [
            {
              name: "Red & Hot",
              desc: "Using a weapon active taints enemies nearby with red paint for 8s and makes them take 25% bonus Physical and Elemental MG (cannot stack). Triggering it again resets the duration",
              priority: "1st",
            },
            {
              name: "Grey & Empty",
              desc: "Enemies stay tainted for 5s longer",
              priority: "2nd",
            },
            {
              name: "White & Bright",
              desc: "Every time an enemy is tainted, Valkyrie restores 12 SP. CD: 5s",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Shine like Stars",
              desc: "When there are enemies tainted with 1/2/3 different paints, Valkyries deal 20%/50%/100% bonus Total DMG to enemies of countering types",
              priority: "CORE",
            },
          ],
        },
      ],
    },
  ],
};
</script>