<template>
    <!-- Main section start -->
	<section class="h-screen px-12 lg:px-32 py-32 mb-8">
		<div class="w-full md:w-1/2 h-full flex flex-col md:justify-center ">
			<!-- Main text start -->
			<h1 class="uppercase text-5xl xl:text-7xl mb-4 font-semibold ">
				房屋的紀錄者
				INTERIOR  PHOTO
			</h1>
			<p class="capitalize xl:w-1/2 text-stone-500">
				居家空間的捕捉者 <br/>
				觀察空間的質感 塑造空間的情感
			</p>
			<div class="flex mt-3 gap-8">
				<a href="#">
					<i class="fa-brands fa-instagram socialIcon"></i>
				</a>
				<a href="#">
					<i class="fa-brands fa-linkedin socialIcon"></i>
				</a>
				<a href="#">
					<i class="fa-brands fa-facebook socialIcon"></i>
				</a>
				<a href="#">
					<i class="fa-brands fa-dribbble socialIcon"></i>
				</a>
				<a href="#">
					<i class="fa-brands fa-pinterest socialIcon"></i>
				</a>
			</div>
		</div>
		<!-- Photographer image start -->
		<div class="absolute bottom-0 right-0 overflow-hidden h-2/5 sm:h-1/2 md:h-3/5 lg:h-4/6 -z-50">
			<img src="@/assets/image.jpg" alt="img" class="h-full">
		</div>
		<div class="w-full h-20 flex justify-start md:justify-center items-center">
			<a href="#about-section">
				<i class="fa-solid fa-arrow-down transition text-stone-100 text-xl bg-yellow-400 rounded-full shadow p-4 hover:-translate-y-2 hover:shadow-xl"></i>
			</a>
		</div>
	</section>
</template>

<script>
export default {

}
</script>

<style>

</style>