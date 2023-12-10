<template>
  <header class="banner overflow-hidden position-relative">
    <NavBar
      class="navBar bg-white"
      :class="{ hidden: isNavBarHidden, 'bg-transparent': isTopScroll }"
    ></NavBar>
    <div class="container pt-20 pt-xl-10">
      <div class="row">
        <div
          class="col-lg-6 d-flex align-items-center justify-content-center justify-content-lg-start mb-4 mb-xl-20"
        >
          <div>
            <p class="fs-12 fs-lg-22 fw-bold mb-4 mb-lg-9" data-aos="fade-right">從喵的眼中</p>
            <p
              class="fs-12 fs-lg-22 fw-bold mb-4 mb-lg-9 text-end"
              data-aos="fade-right"
              data-aos-duration="2000"
            >
              看見台灣
            </p>
            <div class="d-flex" data-aos="fade-right" data-aos-duration="3000">
              <span
                class="px-15 me-6 position-relative"
                style="border-top: 3px solid black; top: 24px"
              ></span>
              <h1 class="h2 me-2">喵立翰</h1>
              <span class="rounded-pill text-bg-secondary_dark fw-medium py-3 px-5"
                >立委候選人</span
              >
            </div>
          </div>
        </div>
        <div class="col-lg-6">
          <div class="d-flex justify-content-center">
            <img src="./assets/img/立委.png" alt="立委" class="main-img" />
          </div>
        </div>
      </div>
    </div>
    <!-- News -->
    <div class="d-none d-lg-flex position-absolute bottom-0 left-0 w-50">
      <div class="d-flex align-items-center bg-secondary_dark">
        <h3 class="h3 text-white ps-25 pe-2">News</h3>
      </div>

      <div class="bg-secondary_light text-white px-4 pe-xl-20 py-4">
        <span>112.12.26</span>
        <p>參與台北寵物論壇，爭取貓咪友善環境</p>
      </div>
      <div class="bg-secondary_dark d-flex flex-column justify-content-center px-2">
        <button type="button" class="up bg-transparent border-0 mb-2"></button
        ><button type="button" class="down bg-transparent border-0"></button>
      </div>
    </div>
  </header>
  <main>
    <RouterView />
  </main>
  <footer>
    <section class="bg-secondary_dark d-flex flex-column align-items-center py-10">
      <h2 class="text-white mb-4">喵立翰競選辦公室</h2>
      <ul class="text-white d-flex mb-8 fs-5">
        <li class="border-end py-sm px-7">首頁</li>
        <li class="border-end py-sm px-7">最新活動</li>
        <li class="border-end py-sm px-7">政策議題</li>
        <li class="py-sm px-7">小額捐款</li>
      </ul>
      <ul class="text-white d-flex flex-column align-items-center fs-5">
        <li class="d-flex mb-3">
          <span class="material-symbols-outlined me-2 fs-9"> location_on </span>
          <p>喵星區，毛茸茸大道88號，喵喵大樓3樓</p>
        </li>
        <li class="d-flex mb-3">
          <span class="material-symbols-outlined me-2 fs-9"> phone_enabled </span>
          <p>(02) 888-5678</p>
        </li>
        <li class="d-flex">
          <span class="material-symbols-outlined me-2 fs-9"> mail </span>
          <p>meowoffice@linmeow.tw</p>
        </li>
      </ul>
    </section>
    <p class="bg-secondary text-center py-5">© 2023 立委候選人喵立翰 版權所有</p>
  </footer>
</template>

<script>
import { RouterView } from 'vue-router'
import NavBar from './components/NavBar.vue'
import { debounce } from 'lodash'
import AOS from 'aos'
import 'aos/dist/aos.css'
export default {
  data() {
    return {
      isNavBarHidden: false,
      lastScrollY: 0,
      isTopScroll: true //滾動條是否在頁面頂部
    }
  },
  components: {
    NavBar,
    RouterView
  },
  methods: {
    handleScroll() {
      // 获取畫面已滚动的像素值即被捲出去的值
      const scrollY = window.pageYOffset
      // 判断滚动方向
      if (scrollY > this.lastScrollY && !this.isNavBarHidden) {
        // 向下滾動，隱藏導航欄
        this.isNavBarHidden = true
      } else if (scrollY < this.lastScrollY && this.isNavBarHidden) {
        // 向上滾動，顯示導航欄
        this.isNavBarHidden = false
      }
      // 更新上次滾動位置
      this.lastScrollY = scrollY
      // 判断是否在頁面頂部
      this.isTopScroll = scrollY === 0
    }
  },
  mounted() {
    window.addEventListener('scroll', debounce(this.handleScroll, 200))
    AOS.init()
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/style/_mixin.scss';
.banner {
  background-image: url('./assets/img/mobile.svg');
  background-size: cover;
  background-position: center center;
  height: 100vh;
  border-radius: 0 0 100px 100px;
  @include lg {
    background-image: url('./assets/img/nav.jpg');
    border-radius: 0 0 200px 200px;
  }
}
.main-img {
  width: 349px;
  @include lg {
    width: 85%;
  }
}
.up {
  background-image: url('./assets/img/up.png');
  background-size: cover;
  background-position: center center;
  width: 24px;
  height: 24px;
}
.down {
  background-image: url('./assets/img/down.png');
  background-size: cover;
  background-position: center center;
  width: 24px;
  height: 24px;
}
.navBar {
  transition: 0.3s ease;
}
.hidden {
  transform: translateY(-100%);
}
</style>
