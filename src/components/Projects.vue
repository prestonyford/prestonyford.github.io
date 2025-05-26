<template>
	<div class="">
		<h1>Projects</h1>
		<div class="mt-4 flex flex-col gap-4">
			<ProjectItem name="Minesweeper" repo="https://github.com/prestonyford/WinXPMinesweeper">
				<template #description>
					<p>
						Minesweeper in the style of Windows XP that runs in the browser.
					</p>
				</template>
				<template #preview>
					<div>
						Hello, world!
					</div>
				</template>
			</ProjectItem>
		</div>
	</div>
</template>

<script setup>
import ProjectItem from './ProjectItem.vue';
</script>
