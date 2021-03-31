<template>
  <div id="app">
    <h1>Hello App!</h1>
    <p>
      <!-- 탐색을 위해 라우터 링크 구성 요소를 사용하십시오. -->
      <!-- `to` prop를 전달하여 링크를 지정하십시오. -->
      <!-- <router-link>는 기본적으로`<a>`태그로 렌더링 될 것입니다 -->
      <router-link to="/">Home</router-link>
      <router-link :to="{ name : 'user', params: { id : 123 }}">/user/123</router-link>
      <router-link to="/user/123">/user/123</router-link>
      <router-link to="/user/asd">/user/asd</router-link>
      <router-link :to="{ name : 'user', params: { id : 'ricky' }}">/user/ricky</router-link>
    </p>
    <!-- route outlet -->
    <!-- 라우트와 일치하는 컴포넌트가 여기 렌더링됩니다. -->
    <router-view></router-view>
  </div>
</template>

<script>
export default {}
</script>

<style>
a {
  color: #42b983;
}
</style>
