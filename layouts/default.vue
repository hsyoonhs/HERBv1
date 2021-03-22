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
      <div class="content container is-max-desktop has-text-grey-light">
        <span style="float: left">개발 및 디자인 ⓒ 2021 Hs Yoon</span>
        <span style="float: right">
          저작권이 명시되지 않은 모든 자료는 청원고등학교에 귀속되어 있습니다.
        </span>
      </div>
    </footer>
  </div>
</template>
