<template>
    <section id="contact-section" class="px-12 lg:px-32 py-16 relative">
        <h1 class="uppercase text-5xl mb-4 font-semibold ">
            團隊 成員
        </h1>
        <div class="grid grid-cols-1 md:grid-cols-2 w-full">
            <div class="hidden md:flex justify-center items-center">
                <img src="@/assets/camera.png" alt="">
            </div>
            <div class="flex flex-col w-full items-start">
                <h1 class="font-bold">wowsite</h1>
                <br>
                <h6 class="text-stone-500">【相關經歷】</h6>
                <p>中興大學、靜宜大學、萬能科大、黎明技術學院/講師</p>
                <p>實踐推廣教育部、勞動部、新北職訓局、信義社大/講師</p>
                <br>
                <h6 class="text-stone-500">【著作】</h6>
                <p>2015Indesign資深設計人講堂 </p>
                <p>2012好攝成癮玩微距</p>
                <p>2010開門撞見大自然</p>
                <p>2008形與色攝影圖文集</p>    
                <br>
                <h6 class="text-stone-500">【攝影展覽】</h6>   
                <p>2020中華攝影藝術交流學會徵件展</p>
                <p>2010台灣生態密碼，攝影聯展</p>
                <p>2010義大利陽光下的形與色</p>
                <br>
                <h6 class="text-stone-500">【雜誌發表】</h6>  
                <p>2009微距攝影下的台北生態日記，頁78-85</p>
                <p>1999面具之下，威尼斯嘉年華，創意檔案雜誌，頁58-63</p>
                <p>1997On Sale，新視界雜誌，頁72</p>                   
            </div>
        </div>        
        <div class="bg-neutral-200 h-44 w-44 md:h-52 md:w-52 rounded-full absolute -top-20 left-0 mt-16 -z-20"></div>
    </section>    
</template>

<script>
export default {
    data() {
        return {
            formData:{
                email:"",
                message:""
            }
        }
    },
    computed: {
        submitValid(){
            return this.formData.email && this.formData.message;
        }
    }

}
</script>

<style>

</style>