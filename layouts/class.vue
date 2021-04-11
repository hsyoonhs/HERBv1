<template>
  <div>
    <header class="class-header">
      <div class="container is-max-desktop">
        <img src="~assets/images/logo.png" />
        <h1 class="title has-text-weight-bold is-size-1">2학년 예반</h1>
        <h2 class="subtitle has-text-weight-bold">청원고교</h2>
      </div>
    </header>
    <nav
      class="navbar header has-shadow is-spaced"
      role="navigation"
      aria-label="main navigation"
    >
      <div class="container is-max-desktop">
        <a class="navbar-item" href="https://school.cbe.go.kr/cw-h"
          >청원고등학교</a
        >
        <a class="navbar-item" href="https://hcs.eduro.go.kr/">자가진단</a>
        <a class="navbar-item" href="https://ebsoc.co.kr/">EBS 온라인클래스</a>
        <a class="navbar-item" href="https://cafe.naver.com/cwhs0501"
          >네이버 카페</a
        >
        <a class="navbar-item" href="https://www.instagram.com/2021_cwhs_/"
          >학생회 인스타</a
        >
        <a
          class="navbar-item"
          href="https://www.youtube.com/channel/UC79aL3O7o-mCNQtbl_C4M0g"
          >학생회 유튜브</a
        >
      </div>
    </nav>

    <nuxt />

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
  </div>
</template>
<style scoped>
.class-header {
  background: linear-gradient(to bottom, transparent, transparent, #dcdcdc);
}

.class-header .container {
  padding: 4rem 0;
  text-align: center;
}

.class-header .container img {
  position: absolute;
  height: 70%;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: -1;
  opacity: 0.2;
  filter: grayscale(1);
}

.class-header .container h1,
.class-header .container h2 {
  text-shadow: 0 0 3px gray;
}

.navbar .container {
  justify-content: center;
}
</style>
