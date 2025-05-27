<template>
	<div class="">
		<h1>Projects</h1>
		<div class="mt-4 flex flex-col gap-8">
			<ProjectItem name="Minesweeper" repo="https://github.com/prestonyford/WinXPMinesweeper">
				<template #description>
					<p>Minesweeper in the style of Windows XP that runs in the browser.</p>
					<p class="mt-4"><b>Tech stack:</b> Vue.js, TypeScript, Tailwind CSS</p>
				</template>
				<template #preview>
					<div class="flex flex-col items-center">
						<iframe src="/minesweeper/index.html" class="w-[246px] h-[338px]"></iframe>
						<div class="flex">
							<BouncyArrow class="w-6 h-6 inline-block rotate-180" />
							<span>Interactive</span>
							<BouncyArrow class="w-6 h-6 inline-block rotate-180" />
						</div>
					</div>
				</template>
			</ProjectItem>
			<ProjectItem name="AudioPlayerWPF" repo="https://github.com/prestonyford/AudioPlayerWPF">
				<template #description>
					<p>An audio player built with .NET's WPF framework that provides several useful features, such as editing tag properties (including album art), creating playlists, creating bookmarks, managing custom starting and ending song positions, and volume control on a per-song basis.</p>
					<p class="mt-4"><b>Tech stack:</b> C#, .NET, WPF (Windows Presentation Foundation)</p>
				</template>
				<template #preview>
					<div class="sm:mt-[2em] w-[246px]">
						<img src="https://raw.githubusercontent.com/prestonyford/AudioPlayerWPF/refs/heads/main/screenshot1.png">
					</div>
				</template>
			</ProjectItem>
			<ProjectItem name="HTTP Cache Parser" repo="https://github.com/prestonyford/http-cache-parser">
				<template #description>
					<p>Inspect the HTTP cache of browsers or online game clients. Searches for media based on their file 
						signatures and strips out other data that would make the file invalid (such as HTTP headers). 
						Preview image or audio assets.</p>
					<p class="mt-4"><b>Tech stack:</b> Node.js, Express.js</p>
				</template>
				<template #preview>
					<div class="sm:mt-[2em] w-[246px]">
						<img src="https://raw.githubusercontent.com/prestonyford/http-cache-parser/refs/heads/master/screenshot2.png">
					</div>
				</template>
			</ProjectItem>
		</div>
	</div>
</template>

<script setup>
import ProjectItem from './ProjectItem.vue';
import BouncyArrow from './BouncyArrow.vue';
</script>
