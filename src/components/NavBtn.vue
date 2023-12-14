<template>
  <!-- 遮罩 -->
  <div class="backdrop d-lg-none" :class="{ 'open-backdrop': isNavOpen }"></div>
  <!-- 漢堡選單 -->
  <a href="#" class="btnNav d-lg-none" @click.prevent="toggleNav" :class="{ open: isNavOpen }">
    <div class="btnLine mb-1"></div>
    <div class="btnLine mb-1"></div>
    <div class="btnLine"></div>
  </a>

  <ul
    class="mobileNav d-flex flex-lg-row align-items-center flex-column pt-20 pt-lg-0"
    :class="{ openNav: isNavOpen }"
  >
    <li class="fw-medium me-8 mb-4 mb-lg-0">
      <RouterLink to="#activity" class="nav-link">最新活動</RouterLink>
    </li>
    <li class="fw-medium me-8 mb-4 mb-lg-0">
      <RouterLink to="#policy" class="nav-link">政策議題</RouterLink>
    </li>
    <li class="fw-medium me-8 d-lg-none">
      <RouterLink to="#donate" class="nav-link">小額捐款</RouterLink>
    </li>
    <li class="d-none d-lg-block">
      <RouterLink class="btn btn-primary rounded-pill py-4 px-9" to="#donate">
        小額捐款
      </RouterLink>
    </li>
  </ul>
</template>

<script>
import { RouterLink } from 'vue-router'
export default {
  data() {
    return {
      isNavOpen: false
    }
  },
  components: {
    RouterLink
  },
  methods: {
    toggleNav() {
      this.isNavOpen = !this.isNavOpen
    },
    //點擊連結時，選單關閉
    navbarCollapse() {
      const navLink = document.querySelectorAll('.nav-link')
      navLink.forEach((item) => {
        item.addEventListener('click', () => {
          this.isNavOpen = false
        })
      })
    }
  },
  mounted() {
    this.navbarCollapse()
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/style/_mixin.scss';
/*漢堡選單*/
.btnNav {
  position: absolute;
  right: 20px;
  width: 45px;
  height: 45px;
  border-radius: 50%;
  padding-left: 12px;
  padding-top: 12px;
  z-index: 3;
  background: #01688c;
}
/*漢堡選單三條線*/
.btnLine {
  border: 2px solid white;
  width: 20px;
  border-radius: 2px;
  transition: 0.3s;
}
@media (max-width: 992px) {
  .mobileNav {
    position: fixed;
    top: 0;
    right: -100%;
    height: 100vh;
    width: 40vw;
    background-color: #f7f7f7;
    z-index: 2;
    display: block;
    transition: 0.3s;
    li a {
      color: black;
    }
  }
}
// 遮罩
.backdrop {
  position: fixed;
  top: 0;
  right: -100%;
  z-index: -1;
  width: 100vw;
  height: 100vh;
  background-color: #000;
  opacity: 0;
  transition: 0.1s;
}
.openNav {
  right: 0;
  display: block;
}
.open-backdrop {
  z-index: 1;
  right: 0;
  opacity: 0.5;
}
//三條線動畫
.btnNav.open .btnLine:nth-child(2) {
  transform: scaleX(0);
  /*   水平尺寸缩放为0，，变得无宽度即隱藏。 */
}

.btnNav.open .btnLine:nth-child(1) {
  /*   transform: rotate(45deg) translate(5px,11px); */
  transform: rotate(135deg) translate(5px, -6px);
}

.btnNav.open .btnLine:nth-child(3) {
  /*   transform: rotate(-45deg) translateY(-6px); */
  transform: rotate(45deg) translate(-4px, -7px);
}
.nav-link:hover {
  color: #01688c;
}
</style>
