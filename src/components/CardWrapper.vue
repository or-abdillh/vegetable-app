<template>
	<section class="wrapper">
		<template v-for="i in 8" :key="i">
			<Card :card="product"></Card>
		</template>
	</section>

</template>

<style scoped>

	.wrapper {
		@apply w-full mt-5 px-5 flex flex-wrap justify-center gap-2;
	}

</style>

 <script setup>

	import Card from './Card.vue'

	const product = {
		image: '/fruit.png',
		name: 'Pineappple',
		category: 'fruit',
		price: '$2.67'
	}

 </script>
