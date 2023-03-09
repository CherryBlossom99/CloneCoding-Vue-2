<template>
  <nav class="navbar navbar-dark bg-dark">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">태연쓰 블로그</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavAltMarkup"
          aria-controls="navbarNavAltMarkup"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
          <div class="navbar-nav">
            <a class="nav-link" aria-current="page" href="#">에이</a>
            <a class="nav-link" href="#">비</a>
            <a class="nav-link" href="#">씨</a>
          </div>
        </div>
      </div>
    </nav>
  </nav>

<router-link to="/list">리스트페이지</router-link>
<router-link to="/">홈페이지</router-link>

<div class="mt-4">
  <router-view :블로그글="블로그글"></router-view>
</div>
  <!-- <ListVue :블로그글="블로그글" /> -->
</template>

<script>
// import ListVue from "./components/List.vue";
import blogdata from "./assets/blog.js";

export default {
  name: "App",
  data() {
    return {
      블로그글: blogdata,
    };
  },
  components: {
    // ListVue,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
