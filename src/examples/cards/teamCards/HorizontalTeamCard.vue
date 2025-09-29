<script setup>
defineProps({
  image: {
    type: String,
    required: true,
  },
  profile: {
    type: Object,
    required: true,
    name: String,
    link: String,
  },
  description: {
    type: String,
    required: true,
  },
  reverse: {
    type: Boolean,
    default: false,
  },
});
</script>
<template>
  <div class="card card-profile team-card">
    <div class="row g-0" :class="{ 'flex-row-reverse': reverse }">
      <div class="col-auto d-flex align-items-center">
        <a :href="profile.link">
          <div class="p-2">
            <img class="shadow-sm" :src="image" :alt="profile.name" />
          </div>
        </a>
      </div>
      <div class="col my-auto">
        <div class="card-body py-2">
          <h5 class="mb-1">{{ profile.name }}</h5>
          <p v-html="description"></p>
        </div>
      </div>
    </div>
  </div>
</template>
<style>
.team-card {
  padding: 15px;
  width: 80%;
  max-width: 1000px;
  margin: 0 auto; /* 水平置中 */
}
.team-card img {
  max-width: 100px; /* 圖片縮小 */
  max-height: 100px;
  object-fit: cover; /* 保持比例 */
  border-radius: 8px;
}
.team-card p {
  font-size: 1rem; /* 文字縮小、簡化 */
  line-height: 1.3;
  color: #555; /* 顏色淺一點 */
  overflow: hidden; /* 避免太長撐高 */
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-box-orient: vertical;
}
</style>
