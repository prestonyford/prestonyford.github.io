<template>
	<div class="flex flex-col sm:flex-row justify-between">
		<div class="">
			<div class="flex sm:items-center sm:gap-4 flex-col sm:flex-row">
				<h3 v-text="name" class="inline grow sm:grow-[initial] basis-0 sm:basis-auto"></h3>
				<Link class="mb-2 sm:mb-0" text="GitHub Repo" :href="repo" target="_blank" :icon="githubIcon"/>
			</div>
			<div>
				<slot name="description"></slot>
			</div>
		</div>

		<div class="ml-2 mt-2 sm:mt-0 flex justify-center sm:justify-start">
			<slot name="preview"></slot>
		</div>
	</div>
</template>

<script setup>
import Link from './Link.vue'
import githubIcon from '@/assets/github-favicon-dark.svg'
</script>

<script>
export default {
	props: ['name', 'repo']
}
</script>
