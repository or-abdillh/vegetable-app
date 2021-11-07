<template>
	<div class="card">
		<i @click="btnLove" class="duration-300 far fa-heart absolute right-2 top-2 text-red-600"></i>
		<img :src="card.image" width="100" class="mx-auto mt-3" />
		<h1 class="text-xs font-bold">{{ card.name }}</h1>
		<p class="text-xs text-gray-400 font-semibold">{{ card.category }}</p>
		<div class="flex justify-between mt-3 items-end">
			<h1 class="text-xs font-semibold text-gray-700">{{ card.price }}</h1>
			<button type="button" class="bg-green text-white rounded px-2 py-1 flex justify-center items-center">
				<i class="fa fa-plus text-xs"></i>
			</button>
		</div>
	</div>
</template>

<style scoped> 

	.card {
		@apply rounded-xl border border-gray-200 p-2 shadow relative;
		width: 45%;
		animation: show .55s ease-in-out forwards;
	}

	@keyframes show {
		from {
			transform: translateY(100%) scale(.5);
			opacity: .75;
		} to {
			transform: translateY(0) scale(1);
			opacity: 1;
		}
	}
	
</style>

<script setup>

	//Define props
	const props = defineProps({
		card: {
			type: Object
		}
	})

    //Handler for love button
    const btnLove = e => {
    	const el = e.target
    	if (el.classList.contains('far')) {
    		el.classList.replace('far', 'fa')
    	} else {
    		el.classList.replace('fa', 'far')
    	}
    }
</script>
