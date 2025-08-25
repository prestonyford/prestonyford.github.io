<template>
	<div>
		<p><b>Tech stack:</b></p>
		<div class="flex flex-wrap gap-2">
			<div v-for="tech in props.stack" class="flex flex-col items-center min-w-[48px]">
				<img :src="techImages[tech]" class="h-[32px]"></img>
				<div>{{ tech }}</div>
			</div>
		</div>
	</div>
</template>

<script setup lang="ts">
import jsLogo from '@/assets/js-logo.png'
import tsLogo from '@/assets/ts-logo.png'
import vueLogo from '@/assets/vue-logo.svg'
import reactLogo from '@/assets/react-logo.png'
import tailwindLogo from '@/assets/tailwind-logo.svg'
import javaLogo from '@/assets/java-logo.png'
import csharpLogo from '@/assets/csharp-logo.png'
import mysql from '@/assets/mysql-logo.png'

type Tech = 'React' | 'Vue.js' | 'TypeScript' | 'JavaScript' | 'TailwindCSS' | 'C#' | '.NET' | 'ASP.NET' | 'WPF' | 'Node.js' | 'Express.js'
const techImages: Record<Tech, string> = {
  React: reactLogo,
  'Vue.js': vueLogo,
  JavaScript: jsLogo,
  TypeScript: tsLogo,
  TailwindCSS: tailwindLogo,
  'C#': csharpLogo,
  '.NET': 'https://upload.wikimedia.org/wikipedia/commons/0/0e/Microsoft_.NET_logo.png',
  'ASP.NET': 'https://upload.wikimedia.org/wikipedia/commons/0/0e/Microsoft_.NET_logo.png',
  'WPF': 'https://upload.wikimedia.org/wikipedia/commons/0/0e/Microsoft_.NET_logo.png',
  'Node.js': 'https://upload.wikimedia.org/wikipedia/commons/d/d9/Node.js_logo.svg',
  'Express.js': 'https://upload.wikimedia.org/wikipedia/commons/6/64/Expressjs.png'
}

const props = defineProps<{
	stack: Tech[]
}>();

</script>