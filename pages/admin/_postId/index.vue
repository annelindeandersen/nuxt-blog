<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
  import AdminPostForm from '@/components/Admin/AdminPostForm';

  export default {
    components: {
      AdminPostForm
    },
    data() {
      return {
        loadedPost: {
          author: 'Anne',
          title: 'My awesome post',
          content: 'Super amazing content',
          thumbnailLink: 'https://static.wixstatic.com/media/b6a0a6_431d6337ed6d43a1b8a91d82a8cb7a1f~mv2.jpg'
        }
      };
    }
  };
</script>

<style lang="css" scoped>
  .update-form {
    width: 90%;
    margin: 20px auto;
  }

  @media (min-width: 768px) {
    .update-form {
      width: 500px;
    }
  }
</style>
