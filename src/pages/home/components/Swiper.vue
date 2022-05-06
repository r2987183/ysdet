<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
            <!-- slides -->
            <swiper-slide>
                <img class="swiper-img" src="https://www.ysdet.tw/images/banner/2_14220211053004.png" />
            </swiper-slide>
            <swiper-slide>
                <img class="swiper-img" src="https://www.ysdet.tw/images/banner/Banner00.jpg" />
            </swiper-slide>
            <swiper-slide>
                <img class="swiper-img" src="https://www.ysdet.tw/images/banner/Banner01.jpg" />
            <!-- Optional controls -->
            <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>
    </div>
</template>

<script>
export default {
    name: 'HomeSwiper',
    data() {
        return {
            swiperOption: {
                pagination: '.swiper-pagination'
            }
        }
    }
}
</script>

<style lang='stylus' scoped>
    .wrapper {
        overflow: hidden
        width: 100%
        height: 0
        padding-bottom: 41.25%
        .swiper-img {
            width: 100%
        }
    }
</style>
