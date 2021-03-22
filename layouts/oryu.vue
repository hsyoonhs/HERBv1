<template>
  <div>
    <section class="hero is-fullheight">
      <div class="hero-body">
        <div class="container is-max-desktop">
          <nuxt />
        </div>
      </div>
      <footer class="footer has-text-grey-lighter">
        <div class="container is-max-desktop">
          <span style="float: left">개발 및 디자인 ⓒ 2021 Hs Yoon</span>
          <span style="float: right">
            저작권이 명시되지 않은 모든 자료는 청원고등학교에 귀속되어 있습니다.
          </span>
        </div>
      </footer>
    </section>
  </div>
</template>
<style scoped>
.hero {
  background: no-repeat center/cover url('~assets/images/error.jpg');
}
.hero-body,
.footer {
  background: transparent;
  backdrop-filter: brightness(0.9);
}
</style>
