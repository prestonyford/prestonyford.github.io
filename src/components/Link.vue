<template>
	<span class="inline-flex">
		<span v-if="icon" class="inline-flex h-[1.5em] items-baseline mr-1 select-none pointer-events-none">
			<img :src="icon" class="max-h-full" />
		</span>
		<a
			class="transition link relative inline-block text-highlight hover:text-highlight-alt"
			:href="href"
			:target="target"
			v-text="text"
		>
		</a>
	</span>
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
		},
		target: {
			type: String,
			default: "_self"
		},
		icon: {
			type: String,
			required: false
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
	bottom: 1px;
	height: 2px;
	width: 0;
	@apply bg-highlight;
}
.link:hover::after {
	width: 100%;
	transition: width 0.2s;
	@apply bg-highlight-alt;
}
</style>