<template>
  <div>
    <div class="post" v-for="post in posts" :key="post">
      <div><strong>Название:</strong> {{ post.title }}</div>
      <div><strong>Описание:</strong> {{ post.body }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    posts: {
      type: Array,
      requierd: true,
    },
  },
};
</script>

<style scoped>
.post {
  border: 2px solid teal;
  margin: 15px auto 0px auto;
}
</style>
