<template>
	<section class="wrapper">
		<template v-for="i in 12" :key="i">
			<Card :card="product"></Card>
		</template>
	</section>

</template>

<style scoped>

	.wrapper {
		@apply w-full mb-24 mt-5 px-5 flex flex-wrap justify-center gap-2;
	}

</style>

 <script setup>

	import Card from './Card.vue'

	const product = {
		image: '/fruit.png',
		name: 'Brocoli',
		category: 'Vegetable',
		price: '$2.67'
	}

 </script>
