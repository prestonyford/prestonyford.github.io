<template>
	<div class="">
		<h1>Projects</h1>
		<div class="mt-4 flex flex-col gap-12">
			<ProjectItem name="Collaborate" repo="https://github.com/prestonyford/collaborate">
				<template #description>
					<p>
						Collaborate is a collaborative teamwork and project management application designed to help
						teams organize work efficiently. It offers an intuitive interface for managing projects,
						columns, and tasks with powerful features like labels, rich text editing, image upload, and
						project sharing.
					</p>
					<TechStack class="my-4" :stack="['React', 'TypeScript', 'TailwindCSS', 'C#', 'ASP.NET']" />
					<div class="grid grid-cols-1 md:grid-cols-2 gap-2 mt-2">
						<img
							src="https://raw.githubusercontent.com/prestonyford/collaborate/refs/heads/main/ss1.png">
						<img
							src="https://raw.githubusercontent.com/prestonyford/collaborate/refs/heads/main/ss2.png">
						<img
							src="https://raw.githubusercontent.com/prestonyford/collaborate/refs/heads/main/ss3.png">
						<img
							src="https://raw.githubusercontent.com/prestonyford/collaborate/refs/heads/main/ss4.png">
					</div>
				</template>
			</ProjectItem>
			<ProjectItem name="WPF Music App" repo="https://github.com/prestonyford/AudioPlayerWPF">
				<template #description>
					<p>An audio player built with .NET's WPF (Windows Presentation Foundation) framework that provides several useful features, such as
						editing tag properties (including album art), creating playlists, creating bookmarks, managing
						custom starting and ending song positions, and volume control on a per-song basis.</p>
					<TechStack class="my-4" :stack="['C#', '.NET', 'WPF']" />
				</template>
				<template #preview>
					<div class="sm:mt-[2em] w-[246px]">
						<img
							src="https://raw.githubusercontent.com/prestonyford/AudioPlayerWPF/refs/heads/main/screenshot1.png">
					</div>
				</template>
			</ProjectItem>
			<ProjectItem name="Minesweeper" repo="https://github.com/prestonyford/WinXPMinesweeper">
				<template #description>
					<p>Minesweeper in the style of Windows XP that runs in the browser. Try it in the demo to the right!
					</p>
					<TechStack class="my-4" :stack="['Vue.js', 'TypeScript', 'TailwindCSS']" />
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
			<ProjectItem name="HTTP Cache Parser" repo="https://github.com/prestonyford/http-cache-parser">
				<template #description>
					<p>Inspect the HTTP cache of browsers or online game clients. Searches for media based on their file
						signatures and strips out other data that would make the file invalid (such as HTTP headers).
						Preview image or audio assets.</p>
					<TechStack class="my-4" :stack="['Node.js', 'Express.js']" />
				</template>
				<template #preview>
					<div class="sm:mt-[2em] w-[246px]">
						<img
							src="https://raw.githubusercontent.com/prestonyford/http-cache-parser/refs/heads/master/screenshot2.png">
					</div>
				</template>
			</ProjectItem>
		</div>
	</div>
</template>

<script setup>
import ProjectItem from './ProjectItem.vue';
import BouncyArrow from './BouncyArrow.vue';
import TechStack from './TechStack.vue';
</script>
