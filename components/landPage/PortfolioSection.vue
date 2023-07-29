<template>
    <!-- Portfolio section start -->
	<section id="portfolio-section" class="px-4 lg:px-8 py-16  relative">
        <!-- Text wrapper start -->
        <div class="flex gap-8 flex-col md:flex-row">
            <h1 class="uppercase text-5xl mb-4 font-semibold ">
                我們的室內影像作品
            </h1>
            <p class="capitalize xl:w-1/2 text-stone-500 mb-8">
                拜訪房子 感受空間 在住的領域探索 思索著空間的本質
            </p>
        </div>
        <!-- Images grid start -->
		<div class="grid-cols-2 md:grid-cols-5 grid mb-8 gap-4">
            <div class="grid grid-cols-1 md:hidden gap-4">
                <img src="@/assets/portfolio/portfolio1.jpg" alt="1" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio2.jpg" alt="2" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio3.jpg" alt="3" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio4.jpg" alt="4" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio5.jpg" alt="5" class="rounded-xl">
            </div>
            <div class="grid grid-cols-1 md:hidden gap-4">
                <img src="@/assets/portfolio/portfolio6.jpg" alt="6" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio7.jpg" alt="7" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio8.jpg" alt="8" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio9.jpg" alt="9" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio10.jpg" alt="10" class="rounded-xl">
            </div>

            <div class="hidden md:flex flex-col gap-4">
                <img src="@/assets/portfolio/portfolio1.jpg" alt="1" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio2.jpg" alt="2" class="rounded-xl">
            </div>
            <div class="hidden md:flex flex-col gap-4">
                <img src="@/assets/portfolio/portfolio3.jpg" alt="1" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio4.jpg" alt="2" class="rounded-xl">
            </div>
            <div class="hidden md:flex flex-col gap-4">
                <img src="@/assets/portfolio/portfolio8.jpg" alt="2" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio5.jpg" alt="2" class="rounded-xl">
            </div>
            <div class="hidden md:flex flex-col gap-4">
                <img src="@/assets/portfolio/portfolio7.jpg" alt="1" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio6.jpg" alt="2" class="rounded-xl">
            </div>
            <div class="hidden md:flex flex-col gap-4">
                <img src="@/assets/portfolio/portfolio9.jpg" alt="1" class="rounded-xl">
                <img src="@/assets/portfolio/portfolio10.jpg" alt="2" class="rounded-xl">
            </div>
        </div>
		<!-- Images grid end -->
        <!-- "More" link start -->
        <a href="https://www.behance.net/WANG81195321" target="_blank" class="text-end">
            <p class="font-semibold text-lg group relative">
                <span>更多室內影像展示 </span>
                <i class="fa-solid fa-arrow-right"></i>
            </p>
        </a>
        <!-- "More" link end -->
        <!-- Circle start -->
        <div class="bg-yellow-400 h-64 w-64 rounded-full absolute top-0 left-0 mt-16 -z-20"></div>
	</section>
</template>

<script>
export default {

}
</script>

<style>

</style>