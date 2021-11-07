<template>
	<section class="fixed shadow-cstm flex justify-between bottom-0 left-0 right-0 bg-white px-3 py-2">
		<template v-for="list in lists" :key="list">
			<div  :class="list.name === 'Search' ? 'text-green-500' : 'text-gray-600'">
				<i :class="list.icon" class="w-full text-base text-center"></i>
				<p class="text-xxs">{{ list.name }}</p>
			</div>
		</template>
	</section>
</template>

<style scoped>

	.text-xxs {
		font-size: .6rem
	}

	.shadow-cstm {
		box-shadow: 4px -1px 12px #BBBBBB;
	}

</style>

<script setup>

	const lists = [
		{
			name: 'Home',
			icon: 'fa fa-home'
		},
		{
			name: 'Search',
			icon: 'fa fa-search'
		},
		{
			name: 'Cart',
			icon: 'fas fa-shopping-cart'
		},
		{
			name: 'Favorite',
			icon: 'far fa-heart'
		},
		{
			name: 'Account',
			icon: 'fa fa-user'
		}
	]

</script>
