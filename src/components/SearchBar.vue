<template>
	<section class="wrapper">
		<div class="bg-secondary search">
			<i class="fa fa-search text-xs mr-3"></i>
			<input v-model="search" type="search" class="bg-secondary focus:outline-none"  placeholder="Input keywords here" />
		</div>
		<i class="fas fa-sliders-h text-gray-700"></i>
	</section>
</template>

<style scoped>

	.wrapper {
		@apply px-5 mt-14 flex justify-between items-center gap-2;
	}

	.search {
		@apply rounded-lg px-3 py-2 w-11/12 text-gray-400;
	}

	input::placeholder, .search {
		font-size: .7rem;
	}

	.-trans-y-50 {
		transform: translateY(-50%);
	}
</style>

<script setup>

	import { ref } from 'vue'

	const search = ref('')

</script>
