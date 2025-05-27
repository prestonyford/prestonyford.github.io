<template>
	<div>
		<!-- <div class="fixed top-[50%] translate-y-[-50%]">
			<TOC class="ml-8" />
		</div> -->
		<div class="mx-auto max-w-4xl pb-[25vh] px-6 lg:px-0">
			<div class="h-screen flex flex-col items-center justify-center">
				<Welcome class="h-full" />
				<div class="relative">
					<BouncyArrow class="w-24 h-24 absolute translate-x-[-50%] bottom-8 cursor-pointer" @click="scrollToExperience" />
				</div>
			</div>
			<div class="flex flex-col gap-24">
				<Experience class="pt-6" ref="experience" />
				<Skills class="" />
				<Projects class="" />
			</div>
		</div>
	</div>
</template>

<script setup>
import TOC from '@/components/TOC.vue'
import Welcome from '@/components/Welcome.vue'
import BouncyArrow from '@/components/BouncyArrow.vue'
import Experience from '@/components/Experience.vue'
import Skills from '@/components/Skills.vue'
import Projects from '@/components/Projects.vue'
</script>

<script>
export default {
	methods: {
		scrollToExperience: function() {
			this.$refs.experience?.$el?.scrollIntoView( { behavior: "smooth", });
		}
	}
}
</script>
