<template>
	<div class="flex flex-col gap-8 items-center justify-center">
		<div class="flex flex-col sm:flex-row gap-4">
			<img alt="Preston Ford" class="rounded-lg object-contain m-auto" src="https://avatars.githubusercontent.com/u/103155705?v=4" height="125" width="125" />
			<div class="flex flex-col gap-2">
				<h2>My name is Preston Ford.</h2>
				<p>
					I'm a Computer Science undergraduate student at BYU. I'm excited at the opportunity
					to enter the field of Software Engineering.
				</p>
			</div>
		</div>
		<div class="flex gap-12">
			<Link text="Download Resume" href="https://drive.google.com/file/d/1J7vuH9CaMzvhEX4PcgUOKD0Fy-D_ZnyJ/view?usp=sharing" target="_blank" />
			<Link text="Contact Me" />
		</div>
	</div>
</template>

<script setup>
import Link from './Link.vue'
</script>
