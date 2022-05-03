<template>
  <div class="">
    <div class="container d-flex justify-content-center align-items-center mt-2">
      <button @click="$router.push('/admin/new-post')" class="btn btn-dark">Yeni Bir Yazı Ekle</button>
    </div>
    <PostList :is-admin="true" />
  </div>
</template>

<script>
import PostList from "@/components/post/PostList.vue";

export default {
  layout: "admin",
  components: {
    PostList,
  },
};
</script>

<style scoped>
</style>