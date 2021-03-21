<template>
  <div>
    <h1 class="title">
      {{ error.statusCode }}
    </h1>
    <h2 v-if="error.statusCode === 404" class="subtitle">
      페이지를 찾을 수 없습니다.
    </h2>
    <h2 v-else class="subtitle">오류가 발생했습니다.</h2>
    <NuxtLink to="/">홈으로 돌아가기</NuxtLink>
  </div>
</template>

<script>
export default {
  props: ['error'],
  layout: 'oryu',
}
</script>
