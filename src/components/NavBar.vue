<template>
  <div class="w-100 position-fixed z-2">
    <div class="container">
      <nav class="d-flex justify-content-between align-items-center py-5">
        <div class="d-flex align-items-end">
          <a class="d-inline-block me-4" href="#" style="width: 150px">
            <img src="@/assets/img/logo.svg" alt="logo" />
          </a>
          <h3 class="fs-5 fw-bold text-primary">Miao Li-Han</h3>
        </div>
        <NavBtn></NavBtn>
      </nav>
    </div>
  </div>
</template>

<script>
import NavBtn from '@/components/NavBtn.vue'
export default {
  components: {
    NavBtn
  }
}
</script>
