<template>
  <div class="home">
    <div>
      <img src="../assets/robot-home.png"
      class="robot"
      aria-hidden="true" />
    </div>

    <div class="get-started">
      <router-link to="/build">Get started</router-link> building your first robot!
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
  created() {
    console.log(process.env.VUE_APP_TEST);
    console.log(process.env.SOME_TEST);
  },
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .home {
    text-align: center;
  }

  .robot {
    height: 300px;
  }
</style>
