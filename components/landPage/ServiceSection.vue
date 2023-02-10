<template>
    <!-- Services section start -->
	<section id="services-section" class="px-12 lg:px-32 py-16 relative overflow-hidden">
        <!-- Text wrapper start -->
        <div class="flex gap-8 flex-col md:flex-row">
            <!-- Main text start -->
            <h1 class="uppercase text-5xl mb-4 font-semibold ">
                我們的服務
            </h1>
            <p class="xl:w-1/2 text-stone-500 mb-8">
                我的專業能幫你做出有質地的影像成品。
                專門協助宅產業類型客戶提供影像製作服務。
                3 個工作天提供您成品，並調整符合到您滿意的狀態。<br/>
                <br/>
                My specialty can help you make textured finished products.
                Specializing in assisting home industry customers to provide video production services.
                3 working days to deliver your finished product and adjust it to your satisfaction.
            </p>

            <!-- Main text end -->
        </div>
        <!-- Text wrapper end -->

        <!-- Services start -->
        <div class="flex flex-col md:flex-row md:gap-8">
            <!-- Wedding service start -->
            <div class="flex flex-row md:flex-col justify-between md:justify-start items-center md:items-start my-8 md:w-1/3">
                <img src="@/assets/services/lifestyle.png" alt="interior" class="-z-50 md:mb-4">
                <div class="w-2/3 text-right md:text-left md:w-full">
                    <nuxt-link to="/photography">
                        <h1 class="uppercase text-2xl font-semibold hover:text-yellow-400 transition delay-80 duration-150 ease-in-out">
                            室內空間商務攝影
                        </h1>
                    </nuxt-link>
                    <p class="capitalize text-stone-500">
                        室內設計事務所完工作品集紀錄
                    </p>
                    <p class="capitalize text-stone-500">
                        Interior Design Office Completed Portfolio Record
                    </p>
                </div>
            </div>
            <!-- Wedding service end -->

            <!-- Wedding service start -->
            <div class="flex flex-row md:flex-col justify-between items-center md:items-start my-8 md:w-1/3">
                <div class="w-2/3 text-left md:w-full md:order-2">
                    <nuxt-link to="/videoCase">
                        <h1 class="uppercase text-2xl font-semibold hover:text-yellow-400 transition delay-80 duration-150 ease-in-out">
                            企業商務影片
                        </h1>
                    </nuxt-link>
                    <p class="capitalize text-stone-500">
                        企業實驗室與工廠動態影片拍攝+剪輯成片
                    </p>
                    <p class="capitalize text-stone-500">                        
                        Corporate dynamic film shooting and editing into film
                    </p>
                </div>
                <img src="@/assets/services/moments.png" alt="film" class="-z-50 md:mb-4 md:order-1">
            </div>
            <!-- Wedding service end -->

            <!-- Wedding service start -->
            <div class="flex flex-row md:flex-col justify-between items-center md:items-start my-8 md:w-1/3">
                <div class="w-1/3">
                    <img src="@/assets/services/home.png" alt="Moments" class="-z-50 md:mb-4">
                </div>
                <div class="w-2/3 text-right md:text-left md:w-full">
                    <nuxt-link to="/familyRecording">
                        <h1 class="uppercase text-2xl font-semibold hover:text-yellow-400 transition delay-80 duration-150 ease-in-out">
                            免費屋主新居落成紀錄片
                        </h1>
                    </nuxt-link>
                    <p class="capitalize text-stone-500">                        
                        免費屋主新屋紀錄片拍攝委託(限台北市)
                    </p>
                    <p class="capitalize text-stone-500">                        
                        Free homeowner's new house record commission (Taipei City)
                    </p>
                </div>
            </div>
            <!-- Wedding service end -->
        </div>
        <!-- Services end -->

        <!-- Circle start -->
        <div class="bg-yellow-400 h-64 w-64 rounded-full absolute top-0 -right-20 mt-16 -z-20"></div>
        <!-- Circle end -->
	</section>
	<!-- Services section end -->
</template>

<script>
export default {

}
</script>

<style>

</style>