<template>
	<div class="flex flex-col gap-8 items-center justify-center">
		<div class="flex flex-col sm:flex-row gap-4">
			<img alt="Preston Ford" class="rounded-lg object-contain m-auto" src="https://avatars.githubusercontent.com/u/103155705?v=4" height="125" width="125" />
			<div class="flex flex-col gap-2">
				<h2>My name is Preston Ford.</h2>
				<p>
					I'm a Computer Science student at BYU with hands-on experience building full-stack web apps. I'm
					passionate about shipping clean, user-focused software—and ready to bring that mindset to the industry.
				</p>
				<p>
					<i>preston.y.ford@gmail.com</i>
				</p>
			</div>
		</div>
		<div class="flex gap-4 sm:justify-center sm:gap-12">
			<Link text="Download Resume" href="Preston Ford Resume.pdf" target="_blank" />
			<Link text="Email Me" href="mailto:preston.y.ford@gmail.com" target="_blank" />
			<Link text="LinkedIn" :icon="linkedinLogo" href="https://www.linkedin.com/in/preston-ford-897761289/" target="_blank" />
		</div>
	</div>
</template>

<script setup>
import Link from '@/components/Link.vue'
import linkedinLogo from '@/assets/linkedin-logo.svg'
</script>
