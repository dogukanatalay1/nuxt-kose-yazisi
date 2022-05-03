<template>
  <div
    class="
      container-fluid
      mt-5
      d-flex
      flex-wrap
      justify-content-center
      align-items-center
    "
  >
    <Post v-for="index in 4" :key="index" :is-admin="isAdmin" />
  </div>
</template>

<script>
import Post from "@/components/post/Post.vue";

export default {
  components: {
    Post,
  },
  props: {
    isAdmin : {
      type: Boolean,
      required: false,
      default: false
    }
  }
};
</script>
