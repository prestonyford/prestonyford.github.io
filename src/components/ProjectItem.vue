<template>
	<div class="flex">
		<div class="grow">
			<div class="flex items-center gap-4">
				<h3 v-text="name" class="inline"></h3>
				<Link text="GitHub Repo" :href="repo" target="_blank" :icon="githubIcon"/>
			</div>
			<div>
				<slot name="description"></slot>
			</div>
		</div>

		<div>
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
