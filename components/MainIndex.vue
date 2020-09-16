<template>
  <div>
    <div class="size">
    <div class="contain_letreiro flex_center_v">
        <!-- Slider main container -->
        <div class="swiper-container swiper-container-horizontal swiper-container-autoheight swiper-container-fade">
            <!-- Additional required wrapper -->
            <div class="swiper-wrapper" style="height: 747px; transition-duration: 0ms;"><div class="swiper-slide swiper-slide-duplicate swiper-slide-duplicate-active" data-swiper-slide-index="2" style="width: 873px; transform: translate3d(0px, 0px, 0px); opacity: 0; transition-duration: 0ms;">
                    <h1 class="title_banner scene_element scene_element--fadeinleft">
                        <span class="nsl margin_tbanner">Almost a decade
                            <br> building brands:</span>
                            <span class="nsb">Over 200 projects
                                <br>of brand identity.</span>
                            </h1>
                        </div>
                <!-- Slides -->



                    <div class="swiper-slide swiper-slide-duplicate-next" data-swiper-slide-index="0" style="width: 873px; transform: translate3d(-873px, 0px, 0px); opacity: 0; transition-duration: 0ms;">
                        <h1 class="title_banner ">
                            <span class="nsl margin_tbanner scene_element scene_element--fadeinleft scene_element--delayed01">A BRAND GOES BEYOND <br>
                            A LOGO DESIGN,</span>
                            <span class="nsb scene_element scene_element--fadeinleft scene_element--delayed02 display-block">IT'S THE RELATIONSHIP BETWEEN<br>
                            PEOPLE AND COMPANIES.</span>
                        </h1>
                    </div>
                    <div class="swiper-slide swiper-slide-prev" data-swiper-slide-index="1" style="width: 873px; transform: translate3d(-1746px, 0px, 0px); opacity: 0; transition-duration: 0ms;">   <h1 class="title_banner scene_element scene_element--fadeinleft">
                        <span class="nsl margin_tbanner">We connect our <br>
                        expertise to yours.</span>
                        <span class="nsb">Together we achieve  <br>
                        rock-solid results.</span>
                    </h1>
                </div>

                <div class="swiper-slide swiper-slide-active" data-swiper-slide-index="2" style="width: 873px; transform: translate3d(-2619px, 0px, 0px); opacity: 1; transition-duration: 0ms;">
                    <h1 class="title_banner scene_element scene_element--fadeinleft">
                        <span class="nsl margin_tbanner">Almost a decade
                            <br> building brands:</span>
                            <span class="nsb">Over 200 projects
                                <br>of brand identity.</span>
                            </h1>
                        </div>

                        <div class="swiper-slide swiper-slide-duplicate swiper-slide-next" data-swiper-slide-index="0" style="width: 873px; transform: translate3d(-3492px, 0px, 0px); opacity: 0; transition-duration: 0ms;">
                        <h1 class="title_banner ">
                            <span class="nsl margin_tbanner scene_element scene_element--fadeinleft scene_element--delayed01">A BRAND GOES BEYOND <br>
                            A LOGO DESIGN,</span>
                            <span class="nsb scene_element scene_element--fadeinleft scene_element--delayed02 display-block">IT'S THE RELATIONSHIP BETWEEN<br>
                            PEOPLE AND COMPANIES.</span>
                        </h1>
                    </div></div>
                        <!-- If we need pagination -->
                        <div class="swiper-pagination scene_element scene_element--fadeinleft scene_element--delayed01 swiper-pagination-clickable swiper-pagination-bullets"><span class="swiper-pagination-bullet"></span><span class="swiper-pagination-bullet"></span><span class="swiper-pagination-bullet swiper-pagination-bullet-active"></span></div>

            <!-- If we need navigation buttons
            <div class="swiper-button-prev"></div>
            <div class="swiper-button-next"></div>-->

            <!-- If we need scrollbar
                <div class="swiper-scrollbar"></div>-->
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'MainIndex',

    data(){
          return
    }
}
</script>
<style>
    .size {
    width: 100%;
    padding: 0 8rem;
    position: relative;
}
</style>
