<template>
	<div>
		<div class="w-screen fixed bg-opacity-90 bg-white p-4 lg:px-20 flex justify-between z-50">
			<!-- Logo start -->
			<nuxt-link to="/" class="h-full flex">
				<img class="h-[50px] mr-2" src="@/assets/logo2.png" alt="" />
				<div class="flex flex-col justify-center">
					<p class="tracking-widest font-semibold text-yellow-400">方生糖</p>
					<p class="tracking-widest font-light">專業空間攝影</p>
				</div>
			</nuxt-link>
			<!-- Logo end -->

			<!-- Toggler start -->
			<button role="menubar" class="md:hidden" @click="navToggle()">
				<i class="fa-solid fa-bars text-2xl"></i>
			</button>
			<!-- Toggler end -->

			<!-- Menu  -->
			<div class="absolute left-0 right-0 translate-y-16 bg-opacity-90 bg-white md:bg-none md:bg-opacity-0 shadow hidden md:flex flex-col gap-4 items-center p-4 md:flex-row md:static md:shadow-none md:translate-y-0"
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
					<a href="https://docs.google.com/forms/d/e/1FAIpQLSf9Gz3Tbm2qxpIxiQVAZRqNx3ZBaO2R3LiQam-Wpyt-xno_kA/viewform" target="_blank" role="menuitem">
						<p class="mx-4">免費新居報名</p>
					</a>		
					<!-- <nuxt-link to="/photography" role="menuitem">
						<p class="mx-4">作品</p>
					</nuxt-link> -->					
					<!-- <nuxt-link to="/familyRecording" role="menuitem">
						<p class="mx-4">免費新居報名</p>
					</nuxt-link> -->
				</template>
				<button class="btn" role="menuitem" @click="showModal = true">
					商業 委託
				</button>
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
}
</style>