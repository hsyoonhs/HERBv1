<template>
  <div>
    <section class="hero is-fullheight">
      <div class="hero-body">
        <div class="container is-max-desktop">
          <nuxt />
        </div>
      </div>
      <footer class="footer">
        <div class="content container is-max-desktop">
          <h3>HERB<sup>v1</sup></h3>
          <li><NuxtLink to="/information">정보</NuxtLink></li>
          <li>개발 및 디자인 ⓒ 2021 Hs Yoon</li>
          <li>
            저작권이 명시되지 않은 모든 자료는 청원고등학교에 귀속되어 있습니다.
          </li>
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
