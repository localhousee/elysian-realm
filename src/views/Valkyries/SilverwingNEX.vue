<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "841657d8-9dbf-4d77-ae23-3efed86503da",
  name: "Silverwing: N-EX",
  imageSrc: "/images/silverwing-nex.png",
  imageAlt: "Silverwing: N-EX",
  position: "object-top",
  derp: {
    imageSrc: "/images/derp/silverwing-nex.png",
    imageAlt: "Derp Silverwing: N-EX",
    position: "object-center",
  }
};

const signets = {
  builds: [
    {
      name: "Recommendation",
      recommended: "Choose Husk",
      boss: "Kalpas",
      supports: [
        {
          time: "Early",
          sigils: "Golden Goblet / Light As a Leaf",
          support_1: "AE",
          support_2: "LE",
        },
        {
          time: "Mid",
          sigils: "Memory / Rainbow Of Absence",
          support_1: "AE",
          support_2: "LE / HB",
        },
        {
          time: "Late",
          sigils: "Home Lost / Dreamful Gold / Empty Like Shala",
          support_1: "AE",
          support_2: "HB",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Grey Falcon",
              desc: "Restores 2 SP per second. Scatter barrier enables Combo ATK and each cast grants 1 stack of Repeating Sequence which costs 7 SP and make Combo ATK deal 16% ATK of bonus Ice DMG. 4 stacks max. Stacks are reset when scatter barrier is removed or created",
              priority: "Start",
            },
            {
              name: "Blessing of Phantom Plumes",
              desc: "After using support skills, tapping [ATK] triggers QTE. QTE boosts Ice DMG by 20% for 30s. 2 stacks max. Triggering it again resets the duration",
              priority: "1st",
            },
            {
              name: "Blessing of Pale Feather",
              desc: "Attacks restore 50% bonus SP. Ultimate deals 2500% ATK of bonus Ice DMG. On hit, Ultimate boosts Elemental Breach by 10% and Total DMG by 45% for 10s. Triggering it again resets the duration",
              priority: "2nd",
            },
            {
              name: "Blessing of Silver Eagle",
              desc: "The last sequence of Basic ATKs restores 2 SP and deals 120% of ATK as bonus Ice DMG. With scatter barrier present, Valkyrie deals 25% bonus Ice DMG and the last sequence of Basic ATKs reduces charging CD by 5s",
              priority: "Filler",
            },
            {
              name: "Blessing of Sharp Eyes",
              desc: "For 10s after landing the Ultimate, Basic ATKs deal 30% of ATK as bonus Ice DMG and Valkyrie restores 25 HP plus 3 SP per second. Triggering it again resets the duration",
              priority: "Filler",
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
              name: "Recitatif of Good Wine",
              desc: "Restore 1.5 SP per second",
              priority: "3rd",
            },
            {
              name: "Recitatif of Fine Jade",
              desc: "Initial SP and max SP increase by 30",
              priority: "Filler",
            },
            {
              name: "Nexus Signet: Echo of Gold",
              desc: "Consuming SP restores the same charges and triggers Final Echo status during which Total DMG increases 8% (160% max) at the cost of charges equal to the remaining duration per second. Insufficient charges reset the effect and end Final Echo",
              priority: "CORE",
            },
            {
              name: "Echo of Withered Soil",
              desc: "After lasting over 7s in Final Note, boost SP cap and restore SP/s till it ends",
              priority: "1st",
            },
            {
              name: "Echo of Silent Night",
              desc: "After lasting over 7s in Final Note, reduce ATK, DEF, ele resists of enemies nearby",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Hua 2",
          lists: [
            {
              name: "Old Dreams Again",
              desc: "Elemental Breach increases by 0.6% per second",
              priority: "1st",
            },
            {
              name: "Dark Garb No More",
              desc: "Elemental DMG increases by 0.8% per second",
              priority: "2nd",
            },
            {
              name: "Long Trip",
              desc: "Total DMG increases by 1.0% per second. 40 stacks max. Taking DMG reduces 10 stacks",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Suffering Mass",
              desc: "Valkyries start with 6 Soldier's Remembrance stacks which boost all buffs from Normal Signets of Vicissitude to full stacks. Taking DMG reduces I Soldier's Remembrance stack and grants 0.5s invincibility",
              priority: "CORE",
            },
            {
              name: "Broken Dream",
              desc: "When possessing Soldier's Remembrance, increase the maximum stack of normal Vicissitude signets by 20",
              priority: "1st",
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
              name: "Nexus Signet: Shine like Stars",
              desc: "When there are enemies tainted with 1/2/3 different paints, Valkyries deal 20%/50%/100% bonus Total DMG to enemies of countering types",
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
              name: "Motto of Pubbe-Nivasanussati",
              desc: "Combo hits are reset at 150 to boost Total DMG by 55% for 10s",
              priority: "Filler",
            },
            {
              name: "Motto of Ceto-Pariya-Nana",
              desc: "Combo hits are reset at 150 to restore 30 SP",
              priority: "Filler",
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