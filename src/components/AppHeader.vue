<template>
  <div class="header">
    <div class="container">
      <div class="logo">logo</div>
      <ul class="text-right">
        <router-link to="" tag="li" exact> <a>Home</a></router-link>

        <router-link to="" tag="li"><a>About</a></router-link>

        <router-link to="/ProjectView" tag="li"
          ><a style="color: burlywood">Projects</a></router-link
        >

        <router-link to="" tag="li"><a>Contact</a></router-link>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style lang="scss" scoped>
.header {
  overflow: hidden;

  .logo {
    font-size: 25px;
    padding: 20px;
    float: left;
    width: 200px;
    color: black;
  }
  ul {
    list-style: none;
    float: left;
    width: calc(100% - 200px);
    li {
      padding: 20px;
      display: inline-block;
      font-size: 18px;

      a {
        text-decoration: none;
        color: black;
      }
    }
  }
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
}
</style>
