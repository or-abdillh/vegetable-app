<template>
	<section class="wrapper">
		<div class="bg-secondary search">
			<i class="fa fa-search text-gray-400 text-xs mr-3"></i>
			<input type="search" class="bg-secondary"  placeholder="Input keywords here" />
		</div>
		<i class="fas fa-sliders-h text-gray-700"></i>
	</section>
</template>

<style scoped>

	.wrapper {
		@apply px-5 mt-16 flex justify-between items-center gap-2;
	}

	.search {
		@apply rounded-lg px-3 py-2 w-11/12;
	}

	input::placeholder, .search {
		font-size: .7rem;
	}

</style>
