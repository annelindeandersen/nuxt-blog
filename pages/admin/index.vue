<template>
  <div class="admin-page">
    <section class="new-post">
      <AppButton @click="$router.push('/admin/new-post')">Create Post</AppButton>
    </section>
    <setion class="existing-posts">
      <h1>Existing posts</h1>
      <PostList isAdmin />
    </setion>
  </div>
</template>

<script>
  import PostList from '@/components/Posts/PostList';
  import AppButton from '@/components/UI/AppButton';

  export default {
    components: {
      PostList,
      AppButton
    }
  };
</script>

<style lang="css" scoped>
  .admin-page {
    padding: 20px;
  }

  .new-post {
    text-align: center;
    border-bottom: 2px solid #ccc;
    padding-bottom: 10px;
  }

  .existing-posts h1 {
    text-align: center;
  }
</style>
