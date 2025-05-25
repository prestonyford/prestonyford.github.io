<template>
	<a
		class="transition px-4 py-2 text-highlight hover:text-highlight-alt"
		:href="href"
	>
		<div class="link relative"
			v-text="text"></div>
	</a>
</template>

<script>
export default {
	props: {
		text: {
			type: String,
			required: true
		},
		href: {
			type: String,
			default: ""
		}
	}
}
</script>

<style scoped>
@reference "../assets/base.css";

a {
	text-decoration: none;
}
.link::after {
	content: "";
	position: absolute;
	display: block;
	height: 2px;
	width: 0;
	@apply bg-highlight;
}
a:hover .link::after {
	width: 100%;
	transition: width 0.2s;
	@apply bg-highlight-alt;
}
</style>