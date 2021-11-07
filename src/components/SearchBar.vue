<template>
	<section class="wrapper">
		<input class="bg-secondary search" typr="search" placeholder="Input keywords here" />
		<i class="fas fa-sliders-h text-gray-700"></i>
	</section>
</template>

<style scoped>

	.wrapper {
		@apply px-5 mt-2 flex justify-between items-center gap-2;
	}

	.search {
		@apply rounded-lg px-3 py-2 w-11/12;
	}

	input::placeholder, .search {
		font-size: .7rem;
	}

</style>
