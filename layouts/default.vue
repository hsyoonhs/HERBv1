<template>
  <div>
    <nav
      class="navbar header has-shadow is-spaced"
      role="navigation"
      aria-label="main navigation"
    >
      <div class="container is-max-desktop">
        <div class="navbar-brand">
          <NuxtLink to="/" class="navbar-item">
            <img src="~assets/logo-text.svg" alt="청원고교" />
          </NuxtLink>
        </div>
      </div>
    </nav>

    <nuxt />

    <footer class="footer">
      <div class="content container is-max-desktop">
        <h2>HERB<sup>v1</sup></h2>
        <li><NuxtLink to="/information">정보</NuxtLink></li>
        <li>개발 및 디자인 ⓒ 2021 Hs Yoon</li>
        <li>
          저작권이 명시되지 않은 모든 자료는 청원고등학교에 귀속되어 있습니다.
        </li>
      </div>
    </footer>
  </div>
</template>
