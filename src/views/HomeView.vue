<template>
  <!-- 我的主張 -->
  <section class="pt-30 pb-30 pb-lg-60">
    <div class="container">
      <div class="row justify-content-center justify-content-lg-between">
        <div class="d-none d-lg-block col-lg-6 position-relative">
          <div data-aos="fade-up">
            <img src="@/assets/img/img2-1.jpg" alt="喵立漢" />
          </div>
          <img
            src="@/assets/img/img2-2.jpg"
            alt="貓咪友善"
            class="position-absolute sec2-img"
            style="top: 120px; left: 170px; z-index: -1"
            data-aos="fade-up"
          />
        </div>
        <div class="col-10 col-lg-4 text-center">
          <h2 class="d-inline-block fw-bold text-primary mb-18 position-relative">
            我的主張
            <span
              class="d-inline-block fs-25 fw-medium text-secondary position-absolute"
              style="top: -53px; left: -20px; z-index: -1"
            >
              c
            </span>
          </h2>
          <p class="mb-6 fs-5 fw-medium">
            我堅信，藉由推動更完善的貓咪福利和相關政策，更是間接地投資於台灣的未來。畢竟，民眾的身心健康與工作熱情是推動經濟的核心動力。透過完善的貓咪福利政策，為台灣的
            GDP 經濟帶來巨大效益。
          </p>
          <p class="fs-5 fw-medium">
            因此，我期望能在立法院內推進這些政策，確保每一隻貓咪都能得到他們應有的照顧，同時也為台灣的經濟發展助一臂之力。讓我們一同護航台灣的幸福經濟，從照顧每一隻貓咪開始。
          </p>
        </div>
      </div>
    </div>
  </section>
  <!-- 最新活動  -->
  <section id="activity" class="sec3-bg py-30 position-relative z-1">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-10">
          <div class="text-center">
            <h2 class="d-inline-block position-relative text-primary fw-bold mb-20">
              最新活動
              <span
                class="d-inline-block fs-25 fw-medium text-white position-absolute"
                style="top: -53px; left: -20px; z-index: -1"
              >
                c
              </span>
            </h2>
          </div>
          <ActivitySwiper class="d-lg-none"></ActivitySwiper>
          <ul class="border position-relative d-none d-lg-block">
            <div class="time-line bg-primary position-absolute"></div>
            <li class="d-flex align-items-center py-9 mb-5" data-aos="fade-up">
              <div
                class="rounded-circle bg-primary h2 py-10 px-2 border border-secondary border-5 text-white me-8"
              >
                12/26
              </div>
              <div class="card bg-transparent border-0">
                <div class="d-flex">
                  <div class="me-6">
                    <img
                      src="@/assets/img/product-01.jpg"
                      class="obj-fit rounded-3"
                      alt="活動照片"
                    />
                  </div>
                  <div class="w-100">
                    <h3 class="mb-4 ps-4">參與台北寵物論壇，爭取貓咪友善環境</h3>
                    <p class="bg-white rounded-3 ps-4 pe-6 py-4">
                      炎炎夏日的周六，我走進了台北寵物論壇，帶著一副貓耳髮箍，決定要全力宣傳「貓咪至上」的理念！我相信，我們的都市中，每一隻貓咪都應該有自己的
                      VIP 休憩空間。
                    </p>
                  </div>
                </div>
              </div>
            </li>
            <li class="d-flex align-items-center py-9 mb-5" data-aos="fade-up">
              <div
                class="rounded-circle bg-primary h2 py-10 px-2 border border-secondary border-5 text-white me-8"
              >
                12/24
              </div>
              <div class="card bg-transparent border-0">
                <div class="d-flex">
                  <div class="me-6">
                    <img
                      src="@/assets/img/product-02.jpg"
                      class="obj-fit rounded-3"
                      alt="活動照片"
                    />
                  </div>
                  <div class="w-100">
                    <h3 class="mb-4 ps-4">掃街模式開啟！帶著你的貓耳，來和我一起走！</h3>
                    <p class="bg-white rounded-3 ps-4 pe-6 py-4">
                      街上氣氛真的很棒，從小孩到大人，甚至有些狗狗朋友都帶著貓耳來找我握手，真的太可愛了！這次的活動不僅讓我看到大家的熱情，更加堅定了我推進「貓咪友善環境」政策的決心。
                    </p>
                  </div>
                </div>
              </div>
            </li>
            <li class="d-flex align-items-center py-9 mb-5" data-aos="fade-up">
              <div
                class="rounded-circle bg-primary h2 py-10 px-2 border border-secondary border-5 text-white me-8"
              >
                12/20
              </div>
              <div class="card bg-transparent border-0">
                <div class="d-flex">
                  <div class="me-6">
                    <img
                      src="@/assets/img/product-03.jpg"
                      class="obj-fit rounded-3"
                      alt="活動照片"
                    />
                  </div>
                  <div class="w-100">
                    <h3 class="mb-4 ps-4">收容所模特兒大比拼！</h3>
                    <p class="bg-white rounded-3 ps-4 pe-6 py-4">
                      今天的收容所不再是一片寂靜。為了讓更多人認識到這裡的毛孩子，我們舉辦了一場前所未有的「模特兒走秀」！
                    </p>
                  </div>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
  <!-- 政策議題 -->
  <section id="policy" class="py-30">
    <div class="container">
      <div class="text-center">
        <h2 class="d-inline-block position-relative text-primary fw-bold mb-20">
          政策議題
          <span
            class="d-inline-block fs-25 fw-medium text-secondary position-absolute"
            style="top: -53px; left: -20px; z-index: -1"
          >
            c
          </span>
        </h2>
      </div>
      <div class="row g-0 justify-content-xxl-center mb-30">
        <div class="col-lg-7 col-xxl-6" data-aos="fade-right">
          <img src="@/assets/img/img4-1.jpg" alt="醫療保障" />
        </div>
        <div
          class="col-lg-7 col-xxl-6 bg-light position-relative policy-right"
          data-aos="fade-left"
        >
          <div class="d-flex justify-content-lg-end pb-9">
            <div class="px-9 pt-6 ps-lg-12 ps-xl-18 pt-lg-12">
              <span class="h3-upline bg-primary mb-2"></span>
              <h3 class="mb-4">推動寵物醫療保障方案</h3>
              <ul>
                <li class="mb-3">
                  ● 提供醫療補助<br />每隻寵物每年可獲得高達新台幣 20,000
                  元的醫療補助，減輕飼主的經濟壓力。
                </li>
                <li class="mb-3">
                  ● 設立寵物醫療基金<br />每年撥款新台幣 10 億元，專款專用於支援家庭寵物的醫療費用。
                </li>
                <li>● 合作動物醫院<br />目前已有和超過 200 家動物醫院進行初步的合作討論。</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <div class="row flex-column-reverse flex-lg-row g-0 justify-content-xxl-center mb-30">
        <div class="col-lg-7 col-xxl-6 bg-light" data-aos="fade-right">
          <div class="d-flex ps-9 pb-9 policy-sec2">
            <div class="pt-6 pt-lg-12">
              <span class="h3-upline bg-primary mb-2"></span>
              <h3 class="mb-4">推廣寵物休閒與娛樂場所</h3>
              <ul class="pe-xl-9">
                <li class="mb-3">
                  ● 建立寵物公園<br />每年撥款新台幣 5
                  億元，用於在各大都市建立專屬的寵物公園。根據初步規劃，預計在第一年內，將在全國範圍內建立至少
                  10 座寵物公園。
                </li>
                <li class="mb-3">
                  ● 推廣寵物友善商家<br />鼓勵商家提供寵物友善的環境，並為參與的商家提供稅收優惠。預計在政策實施後的首年，將有超過
                  500 家商家加入此計畫。
                </li>
                <li>
                  ● 舉辦寵物活動和工作坊<br />與各大寵物社團和組織合作，每年舉辦至少 5
                  場大型的寵物活動，包括寵物才藝比賽、飼養知識工作坊等。
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div
          class="col-lg-7 col-xxl-6 position-relative policy-right ps-0 z-1"
          data-aos="fade-left"
        >
          <img src="@/assets/img/img4-2.jpg" alt="醫療保障" class="obj-fit" />
        </div>
      </div>
      <div class="row g-0 justify-content-xxl-center mb-lg-10">
        <div class="col-lg-7 col-xxl-6" data-aos="fade-right">
          <img src="@/assets/img/img4-3.jpg" alt="醫療保障" />
        </div>
        <div
          class="col-lg-7 col-xxl-6 bg-light position-relative policy-right"
          data-aos="fade-left"
        >
          <div class="d-flex justify-content-end pb-9">
            <div class="px-9 ps-lg-12 ps-xl-18 pt-9 pt-lg-12">
              <span class="h3-upline bg-primary mb-2"></span>
              <h3 class="mb-4">推廣寵物飼養教育</h3>
              <ul>
                <li class="mb-3">
                  ● 建立寵物飼養教育中心<br />每年撥款新台幣 3
                  億元，用於在全國各地建立專業的寵物飼養教育中心。預計在第一年內，在全國至少 5
                  大城市設立教育中心。
                </li>
                <li class="mb-3">
                  ● 推廣寵物飼養課程<br />與學校、社區組織和寵物社團合作，推出一系列免費的寵物飼養課程。預計每年將有超過
                  10,000 名市民受益。
                </li>
                <li>
                  ● 製作教育資料<br />出版寵物飼養手冊、影片和線上課程，讓所有有意飼養寵物的家庭都能輕鬆取得正確的知識。
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- 小額捐款 -->
  <section id="donate" class="py-30 bg-secondary">
    <div class="text-center">
      <h2
        class="d-inline-block position-relative text-primary fw-bold"
        style="z-index: 1; margin-bottom: 170px"
      >
        小額捐款
        <span
          class="d-inline-block fs-25 fw-medium text-white position-absolute"
          style="top: -53px; left: -20px; z-index: -1"
        >
          c
        </span>
      </h2>
      <div class="container">
        <div class="row mb-20">
          <!-- 存錢筒 -->
          <div class="col-lg-6 col-xl-3 mb-30 mb-xl-0 position-relative">
            <div class="d-flex flex-column">
              <div class="position-absolute cat-position">
                <img src="@/assets/img/貓掌.svg" alt="貓掌" />
              </div>
              <div
                class="rounded-4 rounded-bottom-0 bg-secondary_light d-flex flex-column align-items-center py-4"
              >
                <span class="d-block" style="width: 70px; height: 12px; background: #81694a"></span>
                <div class="d-flex align-items-end">
                  <span class="h3 fw-bold text-white me-1">NTD</span>
                  <p class="h2 text-white">600</p>
                </div>
              </div>
              <div class="bg-white py-5 d-flex flex-column align-items-center h-100">
                <span class="fs-5 mb-2">已有</span>
                <div class="d-flex align-items-end">
                  <p class="fs-16 fw-bold me-1">9957</p>
                  <span class="pb-3">人</span>
                </div>
                <span class="fs-5">贊助</span>
              </div>
              <div class="bg-secondary_light py-3">
                <div class="d-flex justify-content-center align-items-center">
                  <span class="me-1"><img src="@/assets/img/Arrow_right.svg" alt="右箭頭" /></span>
                  <p class="text-white fs-6">喵星人之友</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-6 col-xl-3 mb-30 mb-xl-0 position-relative">
            <div class="d-flex flex-column">
              <div class="position-absolute cat-position">
                <img src="@/assets/img/貓掌.svg" alt="貓掌" />
              </div>
              <div
                class="rounded-4 rounded-bottom-0 bg-primary d-flex flex-column align-items-center py-4"
              >
                <span class="d-block" style="width: 70px; height: 12px; background: #015a72"></span>
                <div class="d-flex align-items-end">
                  <span class="h3 fw-bold text-white me-1">NTD</span>
                  <p class="h2 text-white">6,000</p>
                </div>
              </div>
              <div class="bg-white py-5 d-flex flex-column align-items-center h-100">
                <span class="fs-5 mb-2">已有</span>
                <div class="d-flex align-items-end">
                  <p class="fs-16 fw-bold me-1">2000</p>
                  <span class="pb-3">人</span>
                </div>
                <span class="fs-5">贊助</span>
              </div>
              <div class="bg-primary py-3">
                <div class="d-flex justify-content-center align-items-center">
                  <span class="me-1"><img src="@/assets/img/Arrow_right.svg" alt="右箭頭" /></span>
                  <p class="text-white fs-6">喵星大使</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-6 col-xl-3 mb-30 mb-lg-0 position-relative">
            <div class="d-flex flex-column">
              <div class="position-absolute cat-position">
                <img src="@/assets/img/貓掌.svg" alt="貓掌" />
              </div>
              <div
                class="rounded-4 rounded-bottom-0 bg-danger d-flex flex-column align-items-center py-4"
              >
                <span class="d-block" style="width: 70px; height: 12px; background: #772900"></span>
                <div class="d-flex align-items-end">
                  <span class="h3 fw-bold text-white me-1">NTD</span>
                  <p class="h2 text-white">60,000</p>
                </div>
              </div>
              <div class="bg-white py-5 d-flex flex-column align-items-center h-100">
                <span class="fs-5 mb-2">已有</span>
                <div class="d-flex align-items-end">
                  <p class="fs-16 fw-bold me-1">999</p>
                  <span class="pb-3">人</span>
                </div>
                <span class="fs-5">贊助</span>
              </div>
              <div class="bg-danger py-3">
                <div class="d-flex justify-content-center align-items-center">
                  <span class="me-1"><img src="@/assets/img/Arrow_right.svg" alt="右箭頭" /></span>
                  <p class="text-white fs-6">喵星傳奇</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-6 col-xl-3 position-relative">
            <div class="d-flex flex-column h-100">
              <div class="position-absolute cat-position">
                <img src="@/assets/img/貓掌.svg" alt="貓掌" />
              </div>
              <div
                class="rounded-4 rounded-bottom-0 bg-dark d-flex flex-column align-items-center py-4"
              >
                <span class="d-block" style="width: 70px; height: 12px; background: #393939"></span>
                <p class="fs-8 fw-bold text-white">自訂金額</p>
              </div>

              <div
                class="bg-white d-flex justify-content-center align-items-center h-100 py-25 py-lg-0"
              >
                <span class="d-block bg-dark" style="width: 72px; height: 12px"></span>
              </div>
              <div class="bg-dark py-3">
                <div class="d-flex justify-content-center align-items-center">
                  <span class="me-1"><img src="@/assets/img/Arrow_right.svg" alt="右箭頭" /></span>
                  <p class="text-white fs-6">自訂金額</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="d-flex align-items-end">
          <p class="h3 me-4">目前小額贊助總金額：</p>
          <p class="h2 fw-bold">987,655,873</p>
        </div>
      </div>
    </div>
  </section>
  <!-- 民眾服務信箱 -->
  <section>
    <div class="container">
      <div class="row align-items-end">
        <div class="col-lg-6 d-none d-lg-block">
          <div class="position-relative z-1">
            <img src="@/assets/img/立委2.svg" alt="喵立翰立委人像" />
          </div>
        </div>
        <!-- form -->
        <div class="col-lg-7 position-relative form-position" data-aos="fade-up">
          <div class="bg-primary rounded-5 py-30 px-10 px-lg-20">
            <div class="text-center">
              <h2 class="d-inline-block position-relative text-white fw-bold mb-20">
                民眾服務信箱
                <span
                  class="d-inline-block fs-25 fw-medium text-secondary position-absolute"
                  style="top: -53px; left: -20px; z-index: -1"
                >
                  c
                </span>
              </h2>
            </div>
            <form>
              <div class="mb-8 px-8 text-white">
                <label for="name" class="form-label mb-1"
                  ><span class="bg-danger rounded-pill fs-3 px-2 me-1">必填</span>姓名</label
                >
                <input type="text" class="form-control" id="name" />
              </div>
              <div class="mb-8 px-8 text-white">
                <label for="email" class="form-label mb-1"
                  ><span class="bg-danger rounded-pill fs-3 px-2 me-1">必填</span>信箱</label
                >
                <input type="email" class="form-control" id="email" />
              </div>
              <div class="mb-8 px-8 text-white">
                <label for="tel" class="form-label mb-1">手機</label>
                <input type="tel" class="form-control" id="tel" />
              </div>
              <div class="mb-14 px-8 text-white">
                <label for="idea" class="form-label mb-1"
                  ><span class="bg-danger rounded-pill fs-3 px-2 me-1">必填</span>您的建言</label
                >
                <textarea class="form-control" id="idea" rows="6"></textarea>
              </div>
              <div class="d-flex justify-content-center">
                <button
                  type="submit"
                  class="btn btn-outline-light rounded-pill py-4 px-15 fs-5 border-3"
                >
                  送出
                </button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import ActivitySwiper from '@/components/ActivitySwiper.vue'
export default {
  components: {
    ActivitySwiper
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/style/_mixin.scss';
.sec2-img {
  @include lg {
    width: 453px;
  }
  @include xl {
    width: 625px;
  }
}
.sec3-bg {
  background-image: url('@/assets/img/圖樣.jpg');
  position: relative;
  z-index: -2;
}
.time-line {
  width: 6px;
  height: 867px;
  left: 63px;
  z-index: -1;
  @include xl {
    height: 755px;
  }
  @include xxl {
    height: 708px;
  }
}
.policy-right {
  @include lg {
    top: 40px;
    margin-left: -158px;
    padding-left: 158px;
    z-index: -1;
  }

  @include xl {
    margin-left: -194px;
  }
}
.policy-sec2 {
  padding-right: 36px;
  @include lg {
    padding-right: 194px;
  }
}
.h3-upline {
  display: block;
  width: 64px;
  height: 12px;
}
.cat-position {
  top: -66px;
  left: 115px;
  @include md {
    left: 230px;
  }
  @include lg {
    left: 115px;
  }
  @include xl {
    left: 20px;
  }
}
.form-position {
  top: -40px;
  @include lg {
    top: -80px;
    margin-left: -120px;
  }
}
</style>
