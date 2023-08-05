<template>
  <div class="header">
    <div class="container">
      <ul>
        <router-link to="" tag="li" exact>
          <a style="color: burlywood">Web Design</a></router-link
        >

        <router-link to="" tag="li"><a>Mobile App Design</a></router-link>

        <router-link to="" tag="li"><a>Freebies</a></router-link>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "CategoriesMenu",
};
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  color: gray;
}
.header {
  overflow: hidden;
  ul {
    list-style: none;
    color: gray;
    width: calc(100% - 670px);

    li {
      padding: 20px;
      display: inline-block;
      font-size: 20px;

      a {
        text-decoration: none;
        color: gray;
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
