<template>
	<div class="w-24 h-24">
		<svg class="bounce" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
			<g id="SVGRepo_bgCarrier" stroke-width="0"></g>
			<g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
			<g id="SVGRepo_iconCarrier">
				<g id="Arrow / Caret_Down_MD">
					<path id="Vector" d="M16 10L12 14L8 10" stroke="white" stroke-width="2" stroke-linecap="round"
						stroke-linejoin="round"></path>
				</g>
			</g>
		</svg>
	</div>
</template>

<script>
export default {
	props: {

	}
}
</script>

<style scoped>
@keyframes bounce {
	0%,
	40%,
	100% {
		transform: translateY(0);
	}

	20% {
		transform: translateY(18px);
	}
}

.bounce {
	animation: bounce 3s cubic-bezier(0.65, 0, 0.35, 1) infinite;
}
</style>