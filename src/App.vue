<script setup>
import Portfolio from './components/Portfolio.vue'
</script>

<template>
	<header>
	</header>

	<main class="">
		<Portfolio />
	</main>
</template>



<style scoped>
main {
	background-color: #020202;
	
	--dot-color: #1a1a1a;
	--dot-size: 2px;
	--gap: 16px; 
	background-image: radial-gradient(circle at center,
		var(--dot-color) calc(var(--dot-size) / 2),
		transparent calc(var(--dot-size) / 2 + 1px));
	background-size: var(--gap) var(--gap);
	background-attachment: fixed;
}
</style>
