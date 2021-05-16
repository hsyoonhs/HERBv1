<template>
  <div>
    <header class="class-header">
      <div class="container is-max-desktop">
        <img src="~assets/images/logo.png" />
        <hr style="width: 5rem;">
        <h1 class="title has-text-weight-bold is-size-1">2학년 예반</h1>
        <h2 class="subtitle has-text-weight-bold">청원고교</h2>
      </div>
    </header>
    <nav class="navigation">
      <ul>
        <li>
          <a href="https://school.cbe.go.kr/cw-h"> 청원고등학교 </a>
        </li>
        <li>
          <a href="https://hcs.eduro.go.kr/"> 자가진단 </a>
        </li>
        <li>
          <a href="https://ebsoc.co.kr/"> EBS 온라인클래스 </a>
        </li>
        <li>
          <a href="https://www.instagram.com/2021_cwhs_/"> 학생회 인스타 </a>
        </li>
        <li>
          <a href="https://www.youtube.com/channel/UC79aL3O7o-mCNQtbl_C4M0g">
            학생회 유튜브
          </a>
        </li>
      </ul>
    </nav>

    <section class="main-content container is-max-desktop">
      <div class="container column is-10">
        <section class="section">
          <nuxt />
          <div class="columns is-multiline">
            <div class="column">
              <div class="card">
                <header class="card-header">
                  <p class="card-header-title">카드 헤더</p>
                </header>
                <div class="card-content">카드 콘텐츠</div>
              </div>
            </div>
            <div class="column">
              <div class="card">
                <header class="card-header">
                  <p class="card-header-title">카드 헤더</p>
                </header>
                <div class="card-content">카드 콘텐츠</div>
              </div>
            </div>
          </div>
        </section>
      </div>
    </section>

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
  background: #ee9ca7;
  background: -webkit-linear-gradient(to top, #ffdde1, #ee9ca7);
  background: linear-gradient(to bottom, #ffdde1, #ee9ca7);
}

.class-header .container {
  padding: 4rem 0;
  text-align: center;
}

.class-header .container img {
  width: 5rem;
  height: 5rem;
  top: 50%;
  left: 50%;
  filter: invert(1) grayscale(1) brightness(1.9);
}

.class-header .container h1,
.class-header .container h2 {
  text-shadow: 0 0 3px gray;
}

.navigation {
  padding: 0.5rem;
  background-color: #fff;
  border-bottom: 1px solid gainsboro;
  text-align: center;
  white-space: nowrap;
  overflow: auto;
  user-select: none;
  z-index: 1;
}

.navigation li {
  display: inline-block;
}

.navigation a {
  padding: 1rem;
  display: inline-block;
  border-radius: 4px;
  color: darkgray;
  transition: 0.2s;
}

.navigation a:hover {
  background-color: rgba(0, 0, 0, 0.04);
  color: #000;
  filter: none;
}

@media screen and (min-width: 769px) {
  .navigation {
    margin: 0;
    position: sticky;
    top: 0;
  }
}

.navigation::-webkit-scrollbar {
  display: none;
}

.navigation {
  -ms-overflow-style: none;
}
</style>
