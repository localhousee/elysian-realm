<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "f485ba64-cf4d-4729-8c72-834b173e27b0",
  name: "Fervent Tempo",
  imageSrc: "/images/fervent-tempo.png",
  imageAlt: "Fervent Tempo",
  position: "object-right",
  derp: {
    imageSrc: "/images/derp/fervent-tempo.jpg",
    imageAlt: "Derp Fervent Tempo",
    position: "object-center",
  }
};

const signets = {
  builds: [
    {
      name: "1st Variation",
      recommended: "SA for Husk, BR for HoD. Need Sleeper's Dream",
      boss: "Mobius (type advantage)",
      supports: [
        {
          time: "Early",
          sigils: "It Will Be Written",
          support_1: "SA",
          support_2: "SS",
        },
        {
          time: "Mid",
          sigils: "Dreamful Gold",
          support_1: "BR",
          support_2: "SS",
        },
        {
          time: "Late",
          sigils: "Dreamful Gold",
          support_1: "SA/BR",
          support_2: "SS",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Silence",
              desc: "Ultimate CD is reduced 30% and Total DMG dealt is increased 400%. Weapon Active CD is reduced 2s each time Ultimate deals DMG. Strike Back EX is usable during the entirely of Fortress mode",
              priority: "Start",
            },
            {
              name: "Blessing of Thorns",
              desc: "Physical DMG from Basic ATKs (including Charged ATKs) increase 30% and restore 1 SP on hit. At 150 SP, Ultimate cost increase 50 SP. Total DMG dealt by Ultimate increased by 30%",
              priority: "1st",
            },
            {
              name: "Blessing of Solitude",
              desc: "In Fervent Mode, Basic ATKs add 30% ATK of Physical DMG. The last hit of Ultimate adds 300% ATK of Physical DMG",
              priority: "2nd",
            },
            {
              name: "Blessing of Fervor",
              desc: "In Fervent Mode, surrounding enemies take 25% more Physical DMG; Fervent Juice bar is consumed 50% faster (cannot stack)",
              priority: "3rd",
            },
            {
              name: "Blessing of Mixing",
              desc: "Charged ATK and Ultimate draw in enemies within a large radius and increase their Total DMG taken by 40% for 8s. Triggering it again resets the duration",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Eden 2",
          lists: [
            {
              name: "Recitatif of Fine Jade",
              desc: "Initial SP and max SP increase by 30",
              priority: "1st",
            },
            {
              name: "Recitatif of Creeks",
              desc: "Every 10 SP left boosts Physical & Elemental DMG by 2.5%",
              priority: "2nd",
            },
            {
              name: "Recitatif of Good Wine",
              desc: "Restore 1.5 SP per second",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Echo of Gold",
              desc: "Consuming SP restores the same charges and triggers Final Echo status during which Total DMG increases 8% (160% max) at the cost of charges equal to the remaining duration per second. Insufficient charges reset the effect and end Final Echo",
              priority: "CORE",
            },
          ],
        },
        {
          name: "Kevin 1",
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
              name: "Rochet of the Pilgrim",
              desc: "Ultimate restores 3 SP per second for 5s",
              priority: "4th",
            },
            {
              name: "Nexus Signet: Blade of the Deliverer",
              desc: "Ultimate triggers Final Battle status during which all buffs provided by Normal Signets of Deliverance increase by for 5s",
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
          name: "Griseo 2",
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
              name: "Black & Dark",
              desc: "Every time an enemy is tainted, Valkyries deals 10% bonus Physical and Elemental DMG for 20s. 6 stacks max",
              priority: "3rd",
            },
            {
              name: "White & Bright",
              desc: "Every time an enemy is tainted, Valkyrie restores 12 SP. CD: 5s",
              priority: "4th",
            },
            {
              name: "Nexus Signet: Dim Like Stars",
              desc: "?",
              priority: "CORE",
            },
          ],
        },
      ],
    },
    {
      name: "Aponia x Griseo",
      recommended: "Choose Husk. Need Sleeper's Dream. \"Veil of Tears\" can swap to \"Good Old Days\" before Husk. If use Vill-V Core, can use (Faraway Ships & Falling in Past Light). Ref: <a class='italic font-bold underline' href='https://www.youtube.com/watch?v=nQhUmecLWE0'>here</a>",
      boss: "Mobius (type advantage)",
      supports: [
        {
          time: "Early",
          sigils: "Veil of Tears & Boundless Feeling",
          support_1: "VC",
          support_2: "BR",
        },
        {
          time: "Mid",
          sigils: "Veil of Tears & Boundless Feeling",
          support_1: "VC",
          support_2: "BR",
        },
        {
          time: "Late",
          sigils: "(Veil of Tears / Good Old Days) & Boundless Feeling (Read description for Vill-V Core)",
          support_1: "BR",
          support_2: "SS",
        },
      ],
      signets: [
        {
          name: "Elysia",
          info: "double Ego start is a must",
          lists: [
            {
              name: "Blessing of Silence",
              desc: "Ultimate CD is reduced 30% and Total DMG dealt is increased 400%. Weapon Active CD is reduced 2s each time Ultimate deals DMG. Strike Back EX is usable during the entirely of Fortress mode",
              priority: "Start",
            },
            {
              name: "Blessing of Thorns",
              desc: "Physical DMG from Basic ATKs (including Charged ATKs) increase 30% and restore 1 SP on hit. At 150 SP, Ultimate cost increase 50 SP. Total DMG dealt by Ultimate increased by 30%",
              priority: "Start",
            },
            {
              name: "Blessing of Solitude",
              desc: "In Fervent Mode, Basic ATKs add 30% ATK of Physical DMG. The last hit of Ultimate adds 300% ATK of Physical DMG",
              priority: "1st",
            },
            {
              name: "Blessing of Fervor",
              desc: "In Fervent Mode, surrounding enemies take 25% more Physical DMG; Fervent Juice bar is consumed 50% faster (cannot stack)",
              priority: "Filler",
            },
            {
              name: "Blessing of Mixing",
              desc: "Charged ATK and Ultimate draw in enemies within a large radius and increase their Total DMG taken by 40% for 8s. Triggering it again resets the duration",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Aponia 2",
          lists: [
            {
              name: "Fourth, No Insolence",
              desc: "Exhortation increases by 5 per second and caps at 200. Ultimate's Physical and Elemental DMG increases by 0.3% of of Exhortation. Using weapon skills reduces 50% Exhortation",
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
              name: "First, No Betrayal",
              desc: "Exhortation increases by 5 per second and caps at 200. Basic ATK's Total DMG increases by 0.3% of Exhortation. Triggering Ultimate Evasion Skill reduces 50% Exhortation",
              priority: "Optional",
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
              priority: "Filler",
            },
          ],
        },
        {
          name: "Eden 2",
          info: "Build this or Griseo based on RNG Luck. Build this Griseo after this build complete. On 3rd Priority, can take the other one from shop if not have it (Optional)",
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
              name: "Recitatif of Good Wine",
              desc: "Restore 1.5 SP per second",
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
              priority: "YES",
            },
            {
              name: "Echo of Withered Soil",
              desc: "After lasting over 1s, Final Echo boosts SP cap by 50% and restores 1% SP per second until it ends",
              priority: "Optional",
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
              name: "White & Bright",
              desc: "Every time an enemy is tainted, Valkyrie restores 12 SP. CD: 5s",
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
              name: "Fallen Leaves",
              desc: "When yellow and blue taint triggers Blending along with an AoE ATK dealing 800% ATK of Adaptive DMG; CD: 3s. Also taints yourself green for 15s, increasing Total DMG 20% for each taint in Faded Stars. Triggering it again resets the duration",
              priority: "2nd",
            },
          ],
        },
        {
          name: "Su 2 (Choose one)",
          info: "\"Motto of Ceto-Pariya-Nana\" can be paired with \"Withered Soil\"(Eden 2)",
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
              name: "Motto of Ceto-Pariya-Nana",
              desc: "Combo hits are reset at 150 to restore 30 SP",
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
          name: "Kevin 1 (Choose one)",
          lists: [
            {
              name: "Goblet of the Giver",
              desc: "Ultimate boosts Total DMG by 35% for 5s",
              priority: "1st",
            },
            {
              name: "Pendant of the Watcher",
              desc: "Ultimate boosts Physical DMG by 30% for 5s",
              priority: "2nd",
            },
            {
              name: "Rochet of the Pilgrim",
              desc: "Ultimate restores 3 SP per second for 5s",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Blade of the Deliverer",
              desc: "Ultimate triggers Final Battle status during which all buffs provided by Normal Signets of Deliverance increase by for 5s",
              priority: "CORE",
            },
          ],
        },
        {
          name: "Vill-V 1 (Choose one)",
          lists: [
            {
              name: "Act I: Magic",
              desc: "Using a weapon active boosts its Total DMG by 10%. 6 stacks max. Reset at the end of each battle",
              priority: "1st",
            },
            {
              name: "Act II: Pendulum",
              desc: "Using a weapon active makes enemies take 20% bonus Total DMG for 3.5s. Triggering it again resets the duration",
              priority: "2nd",
            },
            {
              name: "Act VI: Sneer",
              desc: "Using a weapon active restores 12 SP in 5s and reduces its CD by 15%",
              priority: "3rd",
            },
            {
              name: "Nexus Signet: Interlude: Reversed Spiral",
              desc: "Using a weapon active unleashes Marvellous Magic dealing 3x400% ATK of Physical DMG to enemies in front and making them take 25% bonus Total DMG for 8s. CDL 5s. The DMG is guaranteed to Crit and the weapon active is the DMG source",
              priority: "CORE",
            },
            {
              name: "Act VIII: Adorned Chamber",
              desc: "Marvellous Magic costs 20 SP to boost its base Physical DMG by 35% and grants 30% Physical Breach for 6s",
              priority: "Filler",
            },
          ],
        },
        {
          name: "Kalpas 2 (Choose one)",
          lists: [
            {
              name: "Blade, Grave, and Scar",
              desc: "Every 100 HP loss boosts Total DMG by 1.0%",
              priority: "1st",
            },
            {
              name: "Bone, Blood, and Ribbon",
              desc: "Every 100 HP loss boosts Physical & Elemental DMG by 0.8%",
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
          name: "Kosma 1 (Choose one)",
          lists: [
            {
              name: "Talons that Desecrate the Santuary",
              desc: "Basic/Combo/Charged ATKs inflict a stack of Rend on hit, each stack dealing 20% ATK of Adaptive DMG per second for 10s. 70 stacks max. Stacking CD: 1s",
              priority: "1st",
            },
            {
              name: "Wings that Mask the Sanguine Moon",
              desc: "Ultimate Evasion Skill inflicts 8 stacks of Rend on all enemies, each stack dealing 20% ATK of Adaptive DMG per second for 70s. 10 stacks max. CD: 8s",
              priority: "2nd",
            },
            {
              name: "Horns that Rip the Bleak Sky",
              desc: "Ultimate inflicts 8 stacks of Rend on all enemies, each stack dealing 20% ATK of Adaptive DMG per second for 10s. 70 stacks max. CD: 8s",
              priority: "3rd",
            },
            {
              name: "Heart that Committed Seven Crimes",
              desc: "Rend lasts 5s longer",
              priority: "Optional",
            },
            {
              name: "Nexus Signet: Daybreak, an Undying Light",
              desc: "Hitting an enemy with 10 or more stacks of Rend triggers Evil's Doom which deals ATK of Adaptive 1500% DMG and 5000% ATK of bonus Adaptive DMG against shields. CD: 5s",
              priority: "CORE",
            },
            {
              name: "Unwavering Promise",
              desc: "Rend-inflicted enemies take 80% bonus Total DMG and addition 40% bonus Total DMG with 20 Rend stacks or more",
              priority: "1st",
            },
          ],
        },
      ],
    },
  ],
};
</script>
