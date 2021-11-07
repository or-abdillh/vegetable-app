<template>
   <!-- Header -->
   <section class="header-wrapper">
      <div class="back-btn">
        <i class="fa fa-chevron-left"></i>
      </div>
      <p class="font-medium text-sm font-semibold">
        Search Items
      </p>
      <div class="user-wrapper">
      	<img src="/user.jpg" width="35" />
      </div>
   </section>
</template>

<style scoped>
   
   .header-wrapper {
      @apply fixed top-0 right-0 left-0 bg-white z-10 w-full mt-1 px-5 py-2 flex justify-between items-center;
   }

   .back-btn {
   	@apply bg-white py-1 px-2 text-gray-600 rounded shadow grid items-center;
   }
   
   .user-wrapper {
      @apply bg-green-500 text-white rounded-full overflow-hidden;
   }
   
</style>
