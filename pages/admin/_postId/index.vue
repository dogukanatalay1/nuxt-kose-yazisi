<template>
  <PostForm :is-update="true" />
</template>

<script>
import PostForm from '@/components/admin/PostForm.vue';

export default {
    components: {
        PostForm
    }
}
</script>