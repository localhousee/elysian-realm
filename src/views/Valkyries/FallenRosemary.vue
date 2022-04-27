<template>
<Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
    import Card from '../../components/Card.vue';

    const valkyrie = {
        id: 4,
        name: 'Fallen Rosemary',
        imageSrc: '/images/fallen-rosemary.jpg',
        imageAlt: 'Fallen Rosemary',
        position: 'object-center',
    };

    const signets = {
        builds: [
            {
                id: 1,
                name: 'Recommendation',
                signets: [
                    {
                        id: 1,
                        name: 'Elysia, rank < SS2',
                        lists: [
                            {
                                id: 1,
                                name: 'Blessing of Nocturne',
                                desc: 'Using God Eater increases Charge ATK TDM',
                                priority: 'Start',
                            },
                            {
                                id: 2,
                                name: 'Blessing of Soul Siphon',
                                desc: 'In Valfreyja form basic ATK siphons extra Disir',
                                priority: '1st',
                            },
                            {
                                id: 3,
                                name: 'Blessing of Valfreyja',
                                desc: 'In Valfreyja form Lightning DMG is increased',
                                priority: '2nd',
                            },
                            {
                                id: 4,
                                name: 'Blessing of God Eater',
                                desc: 'When God Eater hits, a lightning bolt hits and fully recharges Strix',
                                priority: 'Filler',
                            },
                            {
                                id: 5,
                                name: 'Blessing of Spirit Servants',
                                desc: 'When Garmr/Strix/Linnorm hits, increases Lightning DMG',
                                priority: 'Filler',
                            }
                        ],
                    },
                    {
                        id: 2,
                        name: 'Elysia, rank >= SS2',
                        lists: [
                            {
                                id: 1,
                                name: 'Blessing of Nocturne',
                                desc: 'Using God Eater increases Charge ATK TDM',
                                priority: 'Start'
                            },
                            {
                                id: 2,
                                name: 'Blessing of Valfreyja',
                                desc: 'In Valfreyja form Lightning DMG is increased',
                                priority: '1st',
                            },
                            {
                                id: 3,
                                name: 'Blessing of God Eater',
                                desc: 'When God Eater hits, a lightning bolt hits and fully recharges Strix',
                                priority: '2nd',
                            },
                            {
                                id: 4,
                                name: 'Blessing of Soul Siphon',
                                desc: 'In Valfreyja form basic ATK siphons extra Disir',
                                priority: '3rd',
                            },
                            {
                                id: 5,
                                name: 'Blessing of Spirit Servants',
                                desc: 'When Garmr/Strix/Linnorm hits, increases Lightning DMG',
                                priority: 'Filler',
                            }
                        ],
                    },
                    {
                        id: 3,
                        name: 'Su 2',
                        lists: [
                            {
                                id: 1,
                                name: 'Motto of Dibba-Cakkhu',
                                desc: 'Combo hits are reset at to boost Total DMG taken by all enemies by 35% for 10s',
                                priority: '1st'
                            },
                            {
                                id: 2,
                                name: 'Motto of Asavakkhaya',
                                desc: 'Attacks grant 25 bonus combo hits on hit. CD: 5s',
                                priority: '2nd',
                            },
                            {
                                id: 3,
                                name: 'Motto of Iddhi-Vidha',
                                desc: 'Combo hits are increased to 60 when below 60. CD: 10s',
                                priority: '3rd',
                            },
                            {
                                id: 4,
                                name: 'Nexus Signet: Dictum of Bodhi',
                                desc: 'Core',
                                priority: 'Filler',
                            },
                            {
                                id: 5,
                                name: 'Dictum of Anatman',
                                desc: 'The Bodhi: Eyes Open lasts for 3s longer. For every debuff on the target enemy, it takes 5% bonus Total DMG',
                                priority: 'Filler',
                            }
                        ],
                    },
                    {
                        id: 4,
                        name: 'Kevin 1',
                        lists: [
                            {
                                id: 1,
                                name: 'Artifact of the Inhibitor',
                                desc: 'Ultimate boosts Elemental Breach by 20% for 5s',
                                priority: '1st',
                            },
                            {
                                id: 2,
                                name: 'Brand of the Undead',
                                desc: 'Ultimate boosts Elemental DMG by 30% for 5s',
                                priority: '2nd',
                            },
                            {
                                id: 3,
                                name: 'Rochet of the Pilgrim',
                                desc: 'Ultimate restores 3 SP per second for 5s',
                                priority: '3rd',
                            },
                            {
                                id: 4,
                                name: 'Goblet of the Giver',
                                desc: 'Ultimate boosts Total DMG by 35% for 5s',
                                priority: 'Filler',
                            },
                            {
                                id: 5,
                                name: 'Nexus Signet: Blade of the Deliverer',
                                desc: 'Core',
                                priority: '',
                            },
                            {
                                id: 6,
                                name: 'Crusade of the Deliverer',
                                desc: 'After 3s into Final Battle, all buffs provided by Normal Signets of Deliverance increase by 90% instead of 50%',
                                priority: 'YES',
                            },
                            {
                                id: 7,
                                name: 'Echo of the Deliverer',
                                desc: 'Duration of Final Battle and all buffs provided by Normal Signets of Deliverance are extended to 8s',
                                priority: '1st',
                            }
                        ],
                    },
                    {
                        id: 5,
                        name: 'Eden 2',
                        lists: [
                            {
                                id: 1,
                                name: 'Recitatif of Creeks',
                                desc: 'Every 10 SP left boosts Physical & Elemental DMG by 2.5%',
                                priority: '1st',
                            },
                            {
                                id: 2,
                                name: 'Recitatif of Fine Jade',
                                desc: 'Initial SP and max SP increase by 30',
                                priority: '2nd',
                            },
                            {
                                id: 3,
                                name: 'Recitatif of Birds',
                                desc: 'Every 10 SP left reduces Total DMG taken by 2.5%',
                                priority: '3rd',
                            },
                            {
                                id: 4,
                                name: 'Nexus Signet: Echo of Gold',
                                desc: 'Core',
                                priority: '',
                            },
                            {
                                id: 5,
                                name: 'Echo of Silent Night',
                                desc: 'After lasting over 7s, reduce ATK, DEF, ele resists of enemies nearby',
                                priority: 'YES',
                            }
                        ],
                    }
                ]
            }
        ]
    };
</script>
