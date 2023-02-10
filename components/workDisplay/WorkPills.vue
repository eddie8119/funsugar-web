<template>
	<div class="w-screen fixed bg-white z-10">
		<div class="pt-28">
			<div class=" w-full h-20 flex justify-center items-center">
				<nav class="text-stone-500 fixed bg-opacity-90">
					<nuxt-link to="/photography" class="mx-1 md:mx-3 p-4 hover:text-yellow-400 transition delay-80 duration-150 ease-in-out"
						:class="[route === '/photography' ? 'pill-active' : '']">
						室內空間攝影</nuxt-link>
					<nuxt-link to="/videoCase" class="mx-1 md:mx-3 p-4 hover:text-yellow-400 transition delay-80 duration-150 ease-in-out"
						:class="[route === '/videoCase' ? 'pill-active' : '']">
						企業影片製片</nuxt-link>
					<nuxt-link to="/familyRecording" class="mx-1 md:mx-3 p-4 hover:text-yellow-400 transition delay-80 duration-150 ease-in-out"
						:class="[route === '/familyRecording' ? 'pill-active' : '']">
						免費新居婚紗</nuxt-link>
				</nav>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: 'WorkPills',
	data() {
		return {
			nowPath: undefined
		}
	},
	computed: {
		route() {
			return this.$route.path;
		},
	}
}
</script>

<style scoped>
.pill-active {
	@apply text-yellow-400 rounded-full shadow p-4;
}
</style>