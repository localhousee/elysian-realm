<template>
	<a :href="href" class="text-blue-600 hover:underline hover:text-blue-500" target="_blank"><slot /></a>
</template>

<script setup>
defineProps({
	href: String
})
</script>