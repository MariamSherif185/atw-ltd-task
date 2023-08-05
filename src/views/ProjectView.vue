<template>
  <div>
    <div class="title">
      <h1>Our</h1>
      <h1>Projects</h1>
    </div>
    <CategoriesMenu />
    <div class="items">
      <AppItem
        v-for="post in posts"
        :key="post.id"
        :title="post.title"
        :image="post.image"
      />
    </div>
    <div class="down">
      <h3 style="font-weight: bold; color: white; font-size: x-large">
        Interested working with me?
      </h3>
      <button>Email me</button>
    </div>
    <div class="last">
      <h3 style="font-weight: bold; color: black; font-size: x-large">
        Let's Connect
      </h3>
      <div>
        <img src="../assets/instagram.webp" alt="" class="icons" />
        <img src="../assets/youtube.png" alt="" class="icons" />
        <img src="../assets/ball.png" alt="" class="icons" />
      </div>
      <h3 style="font-weight: bold; color: black; font-size: x-large">
        Back to top
      </h3>
    </div>
  </div>
</template>
<script>
import CategoriesMenu from "@/components/CategoriesMenu.vue";
import AppItem from "@/components/AppItem.vue";
import JsonPosts from "../json/json_data.json";
export default {
  data: function () {
    return {
      posts: JsonPosts,
    };
  },
  name: "ProjectView",
  components: {
    CategoriesMenu,
    AppItem,
  },
};
</script>
<style>
.title {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  margin-left: 80px;
}
h1 {
  line-height: 6px;
  color: black;
}
.items {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: center;
}
.down {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  border-radius: 10px;
  width: 75%;
  height: 100px;
  background-color: rgb(237, 160, 59);
  margin-left: 150px;
  margin-top: 40px;
}
.last {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  border-radius: 10px;
  width: 75%;
  height: 100px;
  margin-left: 150px;
  margin-top: 40px;
}
button {
  border-radius: 5px;
  border: 0 solid;
  width: 120px;
  height: 35px;
}
</style>
