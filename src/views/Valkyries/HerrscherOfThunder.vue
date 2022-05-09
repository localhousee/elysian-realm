<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "e8816a8a-39d1-4592-ad31-98d767401df3",
  name: "Herrscher Of Thunder",
  imageSrc: "/images/herrscher-of-thunder.jpg",
  imageAlt: "Herrscher Of Thunder",
  position: "object-top",
};

const signets = {
  builds: [
    {
      name: "4-5",
      supports: [
        {
          time: "Early",
          sigils: "",
          support_1: "AE",
          support_2: "BR",
        },
        {
          time: "Mid",
          sigils: "",
          support_1: "AE",
          support_2: "BR",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "AE",
          support_2: "BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Tsukuyomi",
              desc: "Tap [ATK] after evasion to connect into Basic ATK Sequence 4. Basic ATK Sequence 4 boosts Total DMG by 40% for 5s",
              priority: "Start",
            },
            {
              name: "Blessing of Hazy Moon",
              desc: "Basic ATK Sequence 5 unleashes 3 bolts of thundering sanction each dealing 900% ATK Of Lightning DMG on hit",
              priority: "1st",
            },
            {
              name: "Blessing of Divine Penalty",
              desc: "In burst mode, Bombard costs 200% Herrscher Charge and every hit deals 400% ATK of bonus Lightning DMG",
              priority: "No",
            },
            {
              name: "Blessing of Mitama",
              desc: "Max Herrscher Charge doubles and entering burst mode fully restores it. In burst mode, 75 Herrscher Charge is restored per second. Basic ATK Sequence 5 restores 100 bonus Herrscher Charge",
              priority: "No",
            },
            {
              name: "Blessing of Narukami",
              desc: "Finisher unleashes 8 bolts of Thundering Sanction, each dealing 900% ATK of Lightning DMG on hit",
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
          name: "Pardofelis 1",
          info: "replaced by Aponia 1 (coming soon)",
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
              name: "Lost and Found",
              desc: "Total DMG taken decreases by 0.8% per second",
            },
            {
              name: "Nexus Signet: Suffering Mass",
              desc: "Valkyries start with 6 Soldier's Remembrance stacks which boost all buffs from Normal Signets of Vicissitude to full stacks. Taking DMG reduces I Soldier's Remembrance stack and grants 0.5s invincibility",
              priority: "CORE",
            },
            {
              name: "Worldly Troubles",
              desc: "With Soldier's Remembrance, gain TDM equal to 50% of total damage reduction from signets",
              priority: "1st",
            },
            {
              name: "Broken Dream",
              desc: "When possessing Soldier's Remembrance, increase the maximum stack of normal Vicissitude signets by 20",
              priority: "2nd",
            },
          ],
        },
      ],
    },
    {
      name: "Burst",
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
          support_1: "BR",
          support_2: "LE / BR",
        },
        {
          time: "Late",
          sigils: "",
          support_1: "AE",
          support_2: "BR",
        },
      ],
      signets: [
        {
          name: "Elysia",
          lists: [
            {
              name: "Blessing of Mitama",
              desc: "Max Herrscher Charge doubles and entering burst mode fully restores it. In burst mode, 75 Herrscher Charge is restored per second. Basic ATK Sequence 5 restores 100 bonus Herrscher Charge",
              priority: "Start",
            },
            {
              name: "Blessing of Divine Penalty",
              desc: "In burst mode, Bombard costs 200% Herrscher Charge and every hit deals 400% ATK of bonus Lightning DMG",
              priority: "1st",
            },
            {
              name: "Blessing of Narukami",
              desc: "Finisher unleashes 8 bolts of Thundering Sanction, each dealing 900% ATK of Lightning DMG on hit",
              priority: "2nd",
            },
            {
              name: "Blessing of Tsukuyomi",
              desc: "Tap [ATK] after evasion to connect into Basic ATK Sequence 4. Basic ATK Sequence 4 boosts Total DMG by 40% for 5s",
              priority: "No",
            },
            {
              name: "Blessing of Hazy Moon",
              desc: "Basic ATK Sequence 5 unleashes 3 bolts of thundering sanction each dealing 900% ATK Of Lightning DMG on hit",
              priority: "No",
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
          name: "Pardofelis 1 (Optional)",
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
  ],
};
</script>