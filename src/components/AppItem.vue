<template>
  <div class="item">
    <img :src="image" alt="" class="main-img" />
    <h3 class="post-title">{{ title }}</h3>
    <div class="row">
      <img src="../assets/book.jpg" alt="" class="icons" />
      <span>View Study Case</span>

      <img src="../assets/eye.jpg" alt="" class="icons" />
      <span>Live Preview</span>
    </div>
  </div>
</template>
<script>
export default {
  props: ["title", "image"],
  name: "postT",
};
</script>
<style>
.row {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  width: 50%;
}
.item {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  width: 50%;
  margin-top: 10px;
}
.main-img {
  width: 509px;
  height: 339px;
}
.icons {
  width: 40px;
  height: 40px;
}
</style>
