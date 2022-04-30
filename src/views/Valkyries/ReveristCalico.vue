<template>
<Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from '../../components/Card.vue';

const valkyrie = {
	name: 'Reverist Calico',
	imageSrc: '/images/reverist-calico.jpg',
	imageAlt: 'Reverist Calico',
	position: 'object-[-8rem]',
};

const signets = {
	builds: [
		{
			name: 'Recommendation',
			signets: [
				{
					name: 'Elysia',
					lists: [
						{
							name: 'Blessing of Cat\'s Eyes',
							desc: '',
							priority: 'Start'
						},
						{
							name: 'Blessing of the Tailpiece',
							desc: '',
							priority: 'Start'
						},
						{
							name: 'Blessing of Hidden Claws',
							desc: '',
							priority: '1st'
						},
						{
							name: 'Blessing of Phantasma',
							desc: '',
							priority: '2nd'
						},
						{
							name: 'Blessing of Nighteye',
							desc: '',
							priority: 'Filler'
						},
					],
				},
				{
					name: 'Kevin 1',
					lists: [
						{
							name: 'Artifact of the Inhibitor',
							desc: 'Ultimate boosts Elemental Breach by 25% for 5s',
							priority: '1st'
						},
						{
							name: 'Brand of the Undead',
							desc: 'Ultimate boosts Elemental DMG by 30% for 5s',
							priority: '2nd'
						},
						{
							name: 'Goblet of the Giver',
							desc: 'Ultimate boosts Total DMG by 35% for 5s',
							priority: '3rd'
						},
						{
							name: 'Nexus Signet: Blade of the Deliverer',
							desc: '',
							priority: 'CORE'
						},
						{
							name: 'Crusade of the Deliverer',
							desc: 'After 3s into Final Battle, all buffs provided by Normal Signets of Deliverance increase by 90% instead of 50%',
							priority: '1st'
						},
						{
							name: 'Echo of the Deliverer',
							desc: 'Duration of Final Battle and all buffs provided by Normal Signets of Deliverance are extended to 8s',
							priority: '2nd'
						},
					],
				},
				{
					name: 'Pardofelis 1',
					lists: [
						{
							name: 'Merchant\'s Philosophy',
							desc: 'After finishing each floor, the number of currently owned Shiny Silvers grows by 10% for up to 100 (independent effect)',
							priority: '1st'
						},
						{
							name: 'Shiny & Valuable',
							desc: 'Enemy kills grant bonus Shiny Silvers. Non-boss enemies grant 5 each. Boss enemies grant 100 each (independent effect)',
							priority: '2nd'
						},
						{
							name: 'Back-Curled Tail',
							desc: 'Every 100 Shiny Silvers obtained this round boost Physical and Elemental MG by 0.8%',
							priority: '1st'
						},
						{
							name: 'Flexible P&C',
							desc: 'Every 100 Shiny Silvers obtained this round restore 1 HP and 0.1 SP. Taking DMG disables this effect for 5s',
							priority: 'Optional (Kalpas2 synergy)'
						},
						{
							name: 'Nexus Signet: Empty Dreams, Self, Set, and Joy',
							desc: '',
							priority: 'CORE'
						},
						{
							name: 'This Is Not Where We Die',
							desc: 'Valkyries enters with a Good Luck shield. While the shield holds, every 100 Shiny Silvers owned grant 1% Physical and Elemental Breach. The shield can block incoming MG twice before it breaks, and every 500 Shiny Silvers owned grant one more block',
							priority: 'Optional'
						},
					]
				},
				{
					name: 'Eden 2',
					lists: [
						{
							name: 'Recitatif of Creeks',
							desc: 'Every 10 SP left boosts Physical & Elemental DMG by 2.5%',
							priority: '1st'
						},
						{
							name: 'Recitatif of Eden',
							desc: 'Every 10 SP left boosts Total DMG by 3.0%',
							priority: '2nd'
						},
						{
							name: 'Recitatif of Fine Jade',
							desc: 'Initial SP and max SP increase by 30',
							priority: '3rd'
						},
						{
							name: 'Nexus Signet: Echo of Gold',
							desc: '',
							priority: 'CORE'
						},
						{
							name: 'Echo of Silent Night',
							desc: 'After lasting over 7s, reduce ATK, DEF, ele resists of enemies nearby',
							priority: '1st'
						},
						{
							name: 'Echo of Gold',
							desc: 'After lasting over 7s, boost SP cap and restore SP/s till it ends',
							priority: '2nd'
						},
					],
				},
			]
		}
	]
}
</script>