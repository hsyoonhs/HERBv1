<template>
  <div>
    <section id="main-carousel">
      <b-carousel
        :arrow="arrow"
        :repeat="arrowBoth"
        :arrow-hover="arrowHover"
        :icon-size="iconSize"
      >
        <b-carousel-item class="st-grade">
          <section class="hero">
            <div class="hero-body has-text-centered">
              <h1 class="title is-uppercase has-text-white">
                1<span class="is-size-4">st</span> Grade
              </h1>
              <div class="field has-addons">
                <p class="control">
                  <NuxtLink to="/11">
                    <button class="button">
                      <span>인</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/12">
                    <button class="button">
                      <span>의</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/13">
                    <button class="button">
                      <span>예</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/14">
                    <button class="button">
                      <span>지</span>
                    </button>
                  </NuxtLink>
                </p>
              </div>
              <div class="field has-addons">
                <p class="control">
                  <NuxtLink to="/15">
                    <button class="button">
                      <span>매</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/16">
                    <button class="button">
                      <span>난</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/17">
                    <button class="button">
                      <span>국</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/18">
                    <button class="button">
                      <span>죽</span>
                    </button>
                  </NuxtLink>
                </p>
              </div>
            </div>
          </section>
        </b-carousel-item>
        <b-carousel-item class="nd-grade">
          <section class="hero">
            <div class="hero-body has-text-centered">
              <h1 class="title is-uppercase has-text-white">
                2<span class="is-size-4">nd</span> Grade
              </h1>
              <div class="field has-addons">
                <p class="control">
                  <NuxtLink to="/21">
                    <button class="button">
                      <span>인</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/22">
                    <button class="button">
                      <span>의</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/23">
                    <button class="button">
                      <span>예</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/24">
                    <button class="button">
                      <span>지</span>
                    </button>
                  </NuxtLink>
                </p>
              </div>
              <div class="field has-addons">
                <p class="control">
                  <NuxtLink to="/25">
                    <button class="button">
                      <span>매</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/26">
                    <button class="button">
                      <span>난</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/27">
                    <button class="button">
                      <span>국</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/28">
                    <button class="button">
                      <span>죽</span>
                    </button>
                  </NuxtLink>
                </p>
              </div>
            </div>
          </section>
        </b-carousel-item>
        <b-carousel-item class="rd-grade">
          <section class="hero">
            <div class="hero-body has-text-centered">
              <h1 class="title is-uppercase has-text-white">
                3<span class="is-size-4">rd</span> Grade
              </h1>
              <div class="field has-addons">
                <p class="control">
                  <NuxtLink to="/31">
                    <button class="button">
                      <span>인</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/32">
                    <button class="button">
                      <span>의</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/33">
                    <button class="button">
                      <span>예</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/34">
                    <button class="button">
                      <span>지</span>
                    </button>
                  </NuxtLink>
                </p>
              </div>
              <div class="field has-addons">
                <p class="control">
                  <NuxtLink to="/35">
                    <button class="button">
                      <span>매</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/36">
                    <button class="button">
                      <span>난</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/37">
                    <button class="button">
                      <span>국</span>
                    </button>
                  </NuxtLink>
                </p>
                <p class="control">
                  <NuxtLink to="/38">
                    <button class="button">
                      <span>죽</span>
                    </button>
                  </NuxtLink>
                </p>
              </div>
            </div>
          </section>
        </b-carousel-item>
      </b-carousel>
    </section>
    <section class="main-content container is-max-desktop">
      <div class="container column is-10">
        <section class="section">
          <b-message type="is-info" has-icon>
            개발 단계의 서비스로, 문제가 발생할 수 있습니다.
            <br />
            오류 제보 및 건의는 <code>Not defined</code>로 보내주세요.
          </b-message>
          <div class="columns is-multiline">
            <div class="column is-full">
              <b-collapse
                :open="false"
                class="card"
                animation="slide"
                aria-id="contentIdForA11y3"
              >
                <template #trigger="props">
                  <div
                    class="card-header"
                    role="button"
                    aria-controls="contentIdForA11y3"
                  >
                    <p class="card-header-title">학교 정보</p>
                    <a class="card-header-icon">
                      <b-icon :icon="props.open ? 'menu-up' : 'menu-down'">
                      </b-icon>
                    </a>
                  </div>
                </template>

                <div class="card-content">
                  <div class="content">
                    <p>충북 청주시 청원구 오창읍 구룡5길 9 (28121)</p>
                    <ul>
                      <li>
                        <span class="tag is-primary is-light"
                          >대표(교무실)</span
                        >
                        <a href="tel:043-717-6500">043-717-6500</a>
                      </li>
                      <li>
                        <span class="tag is-warning is-light">FAX</span>
                        <a href="tel:043-717-6509">043-717-6509</a>
                      </li>
                      <li>
                        <span class="tag is-warning is-light">행정실</span>
                        <a href="tel:043-717-6573">043-717-6573</a>
                      </li>
                      <li>
                        <span class="tag is-success is-light"
                          >청심학사(여 · 목령관)</span
                        >
                        <a href="tel:043-717-6591">043-717-6591</a>
                      </li>
                      <li>
                        <span class="tag is-success is-light"
                          >청심학사(남 · 구룡관)</span
                        >
                        <a href="tel:043-717-6594">043-717-6594</a>
                      </li>
                    </ul>
                  </div>
                </div>
                <footer class="card-footer">
                  <a
                    class="card-footer-item"
                    href="https://school.cbe.go.kr/cw-h/M010203/"
                    >학교연혁</a
                  >
                  <a
                    class="card-footer-item"
                    href="https://school.cbe.go.kr/cw-h/M010208/"
                    >교직원 소개</a
                  >
                </footer>
              </b-collapse>
            </div>
            <linkedCard
              to="/meals"
              title="월간 급식"
              icon="food"
              class="main-linkedCard meals"
            >
              이번 달의 급식표 확인하기
            </linkedCard>
            <linkedCard
              to="/teachers"
              title="교사 시간표 (베타)"
              icon="bulletin-board"
              class="main-linkedCard teachers"
            >
              선생님의 일과 살펴보기
            </linkedCard>
          </div>
          <div class="content"></div>
        </section>
      </div>
    </section>
  </div>
</template>
<script>
import linkedCard from '~/components/linkedCard'

export default {
  name: 'HomePage',

  components: {
    linkedCard,
  },

  data() {
    return {
      arrow: true,
      arrowBoth: true,
      arrowHover: true,
      iconSize: 'is-medium',
    }
  },
}
</script>
<style>
.st-grade {
  background: #16bffd;
  background: no-repeat bottom/cover url('~assets/images/banner1.jpg');
}
.nd-grade {
  background: #eecda3;
  background: no-repeat center/cover url('~assets/images/banner2.jpg');
}
.rd-grade {
  background: #4ca1af;
  background: no-repeat top/cover url('~assets/images/banner3.jpg');
}
.st-grade .hero,
.nd-grade .hero,
.rd-grade .hero {
  backdrop-filter: contrast(0.5) grayscale(1) brightness(1.1);
}
.st-grade .title,
.nd-grade .title,
.rd-grade .title {
  font-weight: inherit;
  letter-spacing: 0.1em;
}
.st-grade .field.has-addons,
.nd-grade .field.has-addons,
.rd-grade .field.has-addons {
  justify-content: center;
}
.main-linkedCard .card-header {
  box-shadow: none;
}
.main-linkedCard .card-header-title {
  color: #ffffff;
}
.main-linkedCard .icon {
  color: rgba(255, 255, 255, 0.5) !important;
}
.main-linkedCard .card-footer {
  border: none;
  color: #ffffff;
}
.main-linkedCard .card-footer span {
  background-color: rgba(0, 0, 0, 0.1);
  border-radius: 0.25rem;
  padding: 0.5rem;
}
.main-linkedCard.meals .card {
  background-image: linear-gradient(135deg, #fb7185, #fdba74);
}
.main-linkedCard.teachers .card {
  background-image: linear-gradient(135deg, #818cf8, #d8b4fe, #f9a8d4);
}
</style>
