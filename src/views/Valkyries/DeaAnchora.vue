<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "4678cd4e-07c1-4f1a-b1dd-80aae9eb980e",
  name: "Dea Anchora",
  imageSrc: "/images/dea-anchora.jpg",
  imageAlt: "Dea Anchora",
  position: "object-right-top",
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
          support_2: "MA / BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Stars",
              desc: "Ultimate deals 50% bonus Total DMG",
              priority: "1st",
            },
            {
              name: "Blessing of Halo",
              desc: "Voidstar Anchor, Voidstar Anchor EX, Astral Flares, and Astral Flares EX deal 2000% ATK of Fire DMG to enemies within 8 meters of the target hit, gather them, and restore 50 Astrum. CD: 10s",
              priority: "2nd",
            },
            {
              name: "Blessing of Sheen",
              desc: "Voidstar Anchor EX and Astral Flares EX do not suspend Astrum cosumption, but Seirios Ballista doesnt end Astral Harness and clear Astrum. Seirios Ballista costs 65 SP at most",
              priority: "3rd",
            },
            {
              name: "Blessing of Brilliance",
              desc: "Voidstar Anchor and Astral Flares EX cost no SP and restore 3 SP. Every 30 SP restored deals 800% ATK of Fire DMG to enemies within 10 meters. CD: 6s",
              priority: "Filler",
            },
            {
              name: "Blessing of Gale",
              desc: "In Astral Hamess, all attacks ignite enemies hit and ignited enemies take 25% bonus Total DMG for 10s",
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
              name: "Rochet of the Pilgrim",
              desc: "Ultimate restores 3 SP per second for 5s",
              priority: "3rd",
            },
            {
              name: "Goblet of the Giver",
              desc: "Ultimate boosts Total DMG by 35% for 5s",
              priority: "Filler",
            },
            {
              name: "Nexus Signet: Blade of the Deliverer",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Crusade of the Deliverer",
              desc: "After 3s into Final Battle, all buffs provided by Normal Signets of Deliverance increase by 90% instead of 50%",
              priority: "1st",
            },
            {
              name: "Echo of the Deliverer",
              desc: "Duration of Final Battle and all buffs provided by Normal Signets of Deliverance are extended to 8s",
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
              desc: "Every 10 SP left boost Total DMG by 3.0%",
              priority: "2nd",
            },
            {
              name: "Recitatif of Fine Jade",
              desc: "Initial SP and max SP increase by 30",
              priority: "3rd",
            },
            {
              name: "Recitatif of Birds",
              desc: "Every 10 SP left reduces Total DMG taken by 2.5%",
              priority: "Optional (see Hua)",
            },
            {
              name: "Nexus Signet: Echo of Gold",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Echo of Silent Night",
              desc: "After lasting over 7s, reduce ATK, DEF, ele resists of enemies nearby",
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
              name: "Motto of Dibba-Sota",
              desc: "Combo hits are reset at to reduce Total DMG taken by the Valkyrie by 32% for 10s",
              priority: "Optional (see Hua)",
            },
            {
              name: "Nexus Signet: Dictum of Bodhi",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Dictum of Anatman",
              desc: "Eyes Open debuffs last 3s longer. Every debuff on enemy makes it take 5% more TDM",
              priority: "1st",
            },
            {
              name: "Dictum of Santam",
              desc: "Inflict 3 random debuffs when Eyes Open hit",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Hua 2 (if you choose Total DMG Reduction signets)",
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
              name: "Lost and Found",
              desc: "Total DMG taken decreases by 0.8% per second",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Suffering Mass",
              desc: "",
              priority: "CORE",
            },
            {
              name: "Worldly Troubles",
              desc: "With Soldier's Remembrance, gain TDM equal to 50% of total damage reduction from signets",
              priority: "YES",
            },
            {
              name: "Broken Dream",
              desc: "When possessing Soldier's Remembrance., increase the maximum stack of normal Vicissitude signets by 20",
              priority: "2nd",
            },
          ],
        },
      ],
    },
  ],
};
</script>
