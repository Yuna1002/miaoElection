<template>
  <div class="row">
    <swiper
      :slides-per-view="1.5"
      :spaceBetween="30"
      :centeredSlides="true"
      :pagination="{
        clickable: true
      }"
      :autoplay="{
        delay: 2000,
        disableOnInteraction: false
      }"
      :modules="modules"
      class="pb-12"
    >
      <swiper-slide>
        <div class="card h-100 border-0">
          <img src="@/assets/img/product-01.jpg" class="card-img-top" alt="活動照片" />
          <div class="card-body px-6 pb-6">
            <span class="badge rounded-pill text-bg-primary mb-2">112.12.26</span>
            <h3 class="card-title fs-5 fw-medium">參與台北寵物論壇，爭取貓咪友善環境</h3>
            <p class="card-text">
              炎炎夏日的周六，我走進了台北寵物論壇，帶著一副貓耳髮箍，決定要全力宣傳「貓咪至上」的理念！我相信，我們的都市中，每一隻貓咪都應該有自己的
              VIP 休憩空間。
            </p>
          </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="card h-100 border-0">
          <img src="@/assets/img/product-02.jpg" class="card-img-top" alt="活動照片" />
          <div class="card-body px-6 pb-6">
            <span class="badge rounded-pill text-bg-primary mb-2">112.12.24</span>
            <h3 class="card-title fs-5 fw-medium">掃街模式開啟！帶著你的貓耳，來和我一起走！</h3>
            <p class="card-text">
              街上氣氛真的很棒，從小孩到大人，甚至有些狗狗朋友都帶著貓耳來找我握手，真的太可愛了！這次的活動不僅讓我看到大家的熱情，更加堅定了我推進「貓咪友善環境」政策的決心。
            </p>
          </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="card h-100 border-0">
          <img src="@/assets/img/product-03.jpg" class="card-img-top" alt="活動照片" />
          <div class="card-body">
            <span class="badge rounded-pill text-bg-primary mb-2">112.12.20</span>
            <h3 class="card-title fs-5 fw-medium">收容所模特兒大比拼！</h3>
            <p class="card-text">
              今天的收容所不再是一片寂靜。為了讓更多人認識到這裡的毛孩子，我們舉辦了一場前所未有的「模特兒走秀」！
            </p>
          </div>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from 'swiper/vue'
import { Autoplay, Pagination } from 'swiper/modules'

import 'swiper/css'
import 'swiper/css/pagination'
import 'swiper/css/navigation'

export default {
  components: {
    Swiper,
    SwiperSlide
  },
  setup() {
    return {
      modules: [Autoplay, Pagination]
    }
  }
}
</script>

<style>
.swiper-pagination-bullet-active {
  background: #01688c;
}
</style>
