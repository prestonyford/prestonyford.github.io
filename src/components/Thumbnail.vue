<template>
	<img :src="src" class="cursor-pointer" @click="open" />

	<dialog ref="dialog" class="bg-transparent fixed top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2" @click="onBackdropClick">
		<div class="relative w-[85vw] h-[85vh] m-auto bg-gray-800 border border-gray-500 flex">
			<button
				class="absolute right-0 top-0 px-2 pt-0.5 text-3xl text-gray-100 cursor-pointer bg-gray-800 hover:bg-gray-700 border-b border-l border-gray-500"
				@click="close">
				<i class="fa-solid fa-xmark"></i>
			</button>

			<img :src="src" class="m-auto max-w-full max-h-full cursor-pointer" @click="openImgInNewTab" />
		</div>
	</dialog>
</template>

<script>
export default {
	props: {
		src: {
			type: String,
			required: true
		}
	},
	methods: {
		open() {
			this.$refs.dialog.showModal();
		},
		close() {
			this.$refs.dialog.close();
		},
		onBackdropClick(e) {
			if (e.target === this.$refs.dialog) {
				this.close();
			}
		},
		openImgInNewTab() {
			window.open(this.src, '_blank');
		}
	}
}
</script>

<style scoped>
dialog::backdrop {
	background: rgba(31, 41, 55, 0.6);
}
</style>
