<template>
	<div>
		<div class="w-screen fixed bg-opacity-90 bg-white p-4 lg:px-20 flex justify-between z-50">
			<!-- Logo start -->
			<nuxt-link to="/" class="h-full flex">
				<img class="h-[50px] mr-2" src="@/assets/logo2.png" alt="" />
				<div class="flex flex-col justify-center">
					<p class="tracking-widest font-semibold text-yellow-400">方生糖</p>
					<p class="tracking-widest font-light">室內空間攝影</p>
				</div>
			</nuxt-link>
			<button role="menubar" class="md:hidden" @click="navToggle()">
				<i class="fa-solid fa-bars text-2xl"></i>
			</button>
			<div
				class="absolute left-0 right-0 translate-y-16 bg-opacity-90 bg-white md:bg-none md:bg-opacity-0 shadow hidden md:flex flex-col gap-4 items-center p-4 md:flex-row md:static md:shadow-none md:translate-y-0"
				role="menu" aria-expanded="false">
				<nuxt-link to="/" role="menuitem">
					<p class="mx-4">首頁</p>
				</nuxt-link>
				<template v-if="route === '/'">
					<a href="#services-section" role="menuitem">
						<p class="mx-4">關於</p>
					</a>
					<a href="https://www.behance.net/WANG81195321" target="_blank" role="menuitem">
						<p class="mx-4">作品</p>
					</a>
					<a href="https://pse.is/4r2l4e" target="_blank" role="menuitem">
						<p class="mx-4">新居婚紗</p>
					</a>
					<nuxt-link to="/term-of-service" role="menuitem">
						<p class="mx-4">服務問答</p>
					</nuxt-link>
					<!-- <nuxt-link to="/familyRecording" role="menuitem">
						<p class="mx-4">新居婚紗</p>
					</nuxt-link> -->
				</template>
				<a class="btn" role="menuitem" href="https://mail.google.com/mail/?view=cm&fs=1&to=funsugar8119@gmail.com&body=詢問方生糖:"
					target="_blank">
					攝影預約
				</a>
				<!-- <template v-if="route === '/'">
					<a href="https://www.youtube.com/playlist?list=PLq6qa78AJYu1EK2Ko56KHSnGIjJwmlg4U" target="_blank" role="menuitem">
						<p class="mx-4">引流獲客</p>
					</a>
				</template> -->
			</div>
			<transition name="fade" mode="out-in">
				<div class="modal-overlay absolute w-[120vw] h-[120vh] z-5" v-if="showModal" @click="showModal = false"></div>
			</transition>
			<transition name="fade" mode="out-in" v-if="showModal">
				<CommissionForm />
			</transition>
		</div>
	</div>
</template>

<script>
import CommissionForm from "@/components/Dialog/CommissionForm";

export default {
	name: "Navbar",
	data() {
		return {
			showModal: false,
		};
	},
	components: {
		CommissionForm,
	},
	computed: {
		route() {
			return this.$route.path;
		},
	},
	methods: {
		// Toogle navbar mode 
		navToggle() {
			let menu = document.querySelector("[role='menu']");
			let isExpanded = menu.getAttribute('aria-expanded');
			menu.setAttribute('aria-expanded', !isExpanded);
			menu.classList.toggle('hidden');
			menu.classList.toggle('flex');
		},
	}
}
</script>

<style scoped>
.modal-overlay {
	margin-left: -80px;
	margin-top: -20px;
	background-color: rgba(0, 0, 0, 0.3);
}</style>