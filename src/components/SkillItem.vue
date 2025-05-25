<template>
	<div class="flex flex-col items-center">
		<div class="w-16 h-16">
			<img class="max-h-full m-auto" :src="src" :alt="label" />
		</div>
		<p v-text="label"></p>
	</div>
</template>

<script>
export default {
	props: ['src', 'label']
}
</script>
