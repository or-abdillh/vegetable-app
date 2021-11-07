<template>
    <main class="w-full md:w-8/12 md:mx-auto lg:6/12">
    	<Header></Header>
    	<SearchBar></SearchBar>
	    <CardWrapper></CardWrapper>
    	<Navbar></Navbar>
    </main>
</template>

<script setup>
   
	import Header from './components/Header.vue'
	import SearchBar from './components/SearchBar.vue'
	import CardWrapper from './components/CardWrapper.vue'
	import Navbar from './components/Navbar.vue'
      
</script>
