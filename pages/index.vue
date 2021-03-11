<template>
  <section class="section">
    <div class="columns">
      <card title="Free" icon="github">
        Open source on <a href="https://github.com/buefy/buefy"> GitHub </a>
      </card>

      <card title="Responsive" icon="cellphone-link">
        <b class="has-text-grey"> Every </b> component is responsive
      </card>

      <card title="Modern" icon="alert-decagram">
        Built with <a href="https://vuejs.org/"> Vue.js </a> and
        <a href="http://bulma.io/"> Bulma </a>
      </card>

      <card title="Lightweight" icon="arrange-bring-to-front">
        No other internal dependency
      </card>
    </div>
    <div class="content">
      <ul>
        <li><NuxtLink to="/11">1학년 인반</NuxtLink></li>
        <li><NuxtLink to="/11">1학년 의반</NuxtLink></li>
        <li><NuxtLink to="/11">1학년 예반</NuxtLink></li>
        <li><NuxtLink to="/11">1학년 지반</NuxtLink></li>
        <li><NuxtLink to="/11">1학년 매반</NuxtLink></li>
        <li><NuxtLink to="/11">1학년 난반</NuxtLink></li>
        <li><NuxtLink to="/11">1학년 국반</NuxtLink></li>
        <li><NuxtLink to="/11">1학년 죽반</NuxtLink></li>
        <li><NuxtLink to="/21">2학년 인반</NuxtLink></li>
        <li><NuxtLink to="/22">2학년 의반</NuxtLink></li>
        <li><NuxtLink to="/23">2학년 예반</NuxtLink></li>
        <li><NuxtLink to="/24">2학년 지반</NuxtLink></li>
        <li><NuxtLink to="/25">2학년 매반</NuxtLink></li>
        <li><NuxtLink to="/26">2학년 난반</NuxtLink></li>
        <li><NuxtLink to="/27">2학년 국반</NuxtLink></li>
        <li><NuxtLink to="/28">2학년 죽반</NuxtLink></li>
        <li><NuxtLink to="/31">3학년 인반</NuxtLink></li>
        <li><NuxtLink to="/32">3학년 의반</NuxtLink></li>
        <li><NuxtLink to="/33">3학년 예반</NuxtLink></li>
        <li><NuxtLink to="/34">3학년 지반</NuxtLink></li>
        <li><NuxtLink to="/35">3학년 매반</NuxtLink></li>
        <li><NuxtLink to="/36">3학년 난반</NuxtLink></li>
        <li><NuxtLink to="/37">3학년 국반</NuxtLink></li>
        <li><NuxtLink to="/38">3학년 죽반</NuxtLink></li>
      </ul>
      <ul>
        <li><NuxtLink to="/meals">월간 급식표</NuxtLink></li>
        <li><NuxtLink to="/teachers">교사 시간표</NuxtLink></li>
      </ul>
    </div>
  </section>
</template>

<script>
import Card from '~/components/Card'

export default {
  name: 'HomePage',

  components: {
    Card,
  },
}
</script>
