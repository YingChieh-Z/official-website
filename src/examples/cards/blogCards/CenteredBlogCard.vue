<script setup>
defineProps({
  image: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  description: {
    type: String,
    required: true,
  },
  action: {
    type: Object,
    color: String,
    route: String,
    label: String,
    default: () => ({
      color: "bg-gradient-success",
      label: "Find Out More",
    }),
  },
});
</script>
<template>
  <div class="card">
    <div
      class="card-header p-0 position-relative mt-n4 mx-3 z-index-2 text-center"
    >
      <a :href="action.route" class="d-inline-block blur-shadow-image">
        <img :src="image" :alt="title" class="centered-blog-card-img" />
      </a>
    </div>
    <div class="card-body text-center">
      <h5 class="font-weight-normal">
        <a href="javascript:;">{{ title }}</a>
      </h5>
    </div>
  </div>
</template>
<style>
.centered-blog-card-img {
  width: 200px; /* 固定寬度 */
  height: 200px; /* 固定高度 */
  object-fit: cover; /* 保持比例，裁切多餘部分 */
  border-radius: 12px; /* 可選：圓角 */
  margin: 0 auto; /* 水平置中 */
  display: block;
}
</style>
