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
          <div class="columns">
            <linkedCard to="/meals" title="월간 급식" icon="food">
              이번 달의 급식표 확인하기
            </linkedCard>
            <linkedCard
              to="/teachers"
              title="교사 시간표 (베타)"
              icon="bulletin-board"
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
  background: -webkit-linear-gradient(to right, #cb3066, #16bffd);
  background: linear-gradient(to right, #cb3066, #16bffd);
}
.nd-grade {
  background: #eecda3;
  background: -webkit-linear-gradient(to right, #ef629f, #eecda3);
  background: linear-gradient(to right, #ef629f, #eecda3);
}
.rd-grade {
  background: #4ca1af;
  background: -webkit-linear-gradient(to right, #c4e0e5, #4ca1af);
  background: linear-gradient(to right, #c4e0e5, #4ca1af);
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
</style>
