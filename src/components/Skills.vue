<template>
	<div class="">
		<h1>Skills</h1>
		<div class="mt-4 grid grid-cols-4 md:grid-cols-8 gap-4">
			<SkillItem :src="jsLogo" label="JavaScript"/>
			<SkillItem :src="tsLogo" label="TypeScript"/>
			<SkillItem :src="vueLogo" label="Vue.js"/>
			<SkillItem :src="reactLogo" label="React"/>
			<SkillItem :src="javaLogo" label="Java"/>
			<SkillItem :src="csharpLogo" label="C#"/>
			<SkillItem :src="mysql" label="MySQL"/>
			<SkillItem :src="gitLogo" label="Git"/>
		</div>
	</div>
</template>

<script setup>
import SkillItem from './SkillItem.vue';
import jsLogo from '@/assets/js-logo.png'
import tsLogo from '@/assets/ts-logo.png'
import vueLogo from '@/assets/vue-logo.svg'
import reactLogo from '@/assets/react-logo.png'
import javaLogo from '@/assets/java-logo.png'
import csharpLogo from '@/assets/csharp-logo.png'
import mysql from '@/assets/mysql-logo.png'
import gitLogo from '@/assets/git-logo.png'
</script>
