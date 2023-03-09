<template>
  <div>
    <h4 @click="$router.push('/detail/0')">{{ 블로그글[0].title }}</h4>
    <p>{{ 블로그글[0].date }}</p>
  </div>
  <div>
    <h4>{{ 블로그글[1].title }}</h4>
    <p>{{ 블로그글[1].date }}</p>
  </div>
  <div>
    <h4>{{ 블로그글[2].title }}</h4>
    <p>{{ 블로그글[2].date }}</p>
  </div>
  <button type="button" class="btn btn-primary" @click="$router.go(-1)">뒤로가기</button>
</template>

<script>
export default {
  name: "list",
  props: {
    블로그글: Array,
  },
};
</script>

<style>
</style>