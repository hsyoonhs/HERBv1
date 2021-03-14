<template>
  <div>
    <nav
      class="navbar header has-shadow is-spaced"
      role="navigation"
      aria-label="main navigation"
    >
      <div class="container is-max-desktop">
        <div class="navbar-brand">
          <a class="navbar-item" href="/">
            <h1 class="title is-4 has-text-weight-bold">HERBv1</h1>
          </a>
        </div>
      </div>
    </nav>

    <section class="main-content container is-max-desktop">
      <aside class="column is-2 section">
        <p class="menu-label is-hidden-touch">General</p>
        <ul class="menu-list">
          <li v-for="(item, key) of items" :key="key">
            <nuxt-link :to="item.to" exact-active-class="is-active">
              <b-icon :icon="item.icon" /> {{ item.title }}
            </nuxt-link>
          </li>
        </ul>
      </aside>

      <div class="container column is-10">
        <nuxt />
      </div>
    </section>

    <footer class="footer">
      <div class="content container is-max-desktop has-text-grey-light">
        <p>
          개발 및 디자인 ⓒ 2021 Hs Yoon
          <br>
          저작권이 명시되지 않은 모든 자료는 청원고등학교에 귀속되어 있습니다.
        </p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: '홈',
          icon: 'home',
          to: { name: 'index' },
        },
        {
          title: '영감',
          icon: 'lightbulb',
          to: { name: 'inspire' },
        },
      ],
    }
  },
}
</script>
