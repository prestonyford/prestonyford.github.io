<template>
	<div class="grid grid-cols-2 items-end">
		<h3 v-text="position"></h3>
		<span class="text-right" v-text="date"></span>
		<i v-text="company"></i>
		<span class="text-right self-start" v-text="location"></span>
		<div class="col-span-full pt-1">
			<slot></slot>
		</div>
	</div>
</template>

<script>
export default {
	props: ["position", "company", "date", "location"]
}
</script>
