<template>
<fragment>
  <Header/>
  <div class="content-wrapper">
    <Nuxt />
  </div>
</fragment>
</template>

<script>
  import Header from "../components/Header";
  import Fragment from 'vue-fragment';
  import Vue from "vue";
  Vue.use(Fragment.Plugin);
  export default {
    components: {Header}
  }
</script>

<style>
  html {
    font-family:
      'Source Sans Pro',
      -apple-system,
      BlinkMacSystemFont,
      'Segoe UI',
      Roboto,
      'Helvetica Neue',
      Arial,
      sans-serif;
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
  }

  *,
  *::before,
  *::after {
    box-sizing: border-box;
    margin: 0;
  }

  .content-wrapper {
    background: #f6f6f6;
    color: #444;
  }

  .button--green {
    display: inline-block;
    border-radius: 4px;
    border: 1px solid #3b8070;
    color: #3b8070;
    text-decoration: none;
    padding: 10px 30px;
  }

  .button--green:hover {
    color: #fff;
    background-color: #3b8070;
  }

  .button--grey {
    display: inline-block;
    border-radius: 4px;
    border: 1px solid #35495e;
    color: #35495e;
    text-decoration: none;
    padding: 10px 30px;
    margin-left: 15px;
  }

  .button--grey:hover {
    color: #fff;
    background-color: #35495e;
  }

  .flex-wrap {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
  }

  .page-title {
    margin-bottom: 20px;
  }

  .button {
    display: flex;
    background: white;
    border: 1px solid white;
    padding: 10px 50px;
    min-width: 58px;
  }
</style>
