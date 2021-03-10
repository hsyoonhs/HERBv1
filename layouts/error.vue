<template>
  <div>
    <h1 v-if="error.statusCode === 404">페이지를 찾을 수 없습니다.</h1>
    <h1 v-else>오류가 발생했습니다.</h1>
    <NuxtLink to="/">홈으로 돌아가기</NuxtLink>
  </div>
</template>

<script>
  export default {
    props: ['error'],
    layout: 'error' // you can set a custom layout for the error page
  }
</script>