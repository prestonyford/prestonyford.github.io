<template>
	<div class="grid grid-cols-2 items-end">
		<h4 v-text="position"></h4>
		<span class="text-right" v-text="date"></span>
		<span v-text="company"></span>
		<span class="text-right" v-text="location"></span>
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
