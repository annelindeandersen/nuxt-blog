<template>
  <section class="featured-posts">
    <PostPreview
      :is-admin="isAdmin"
      id="1"
      thumbnail="https://static.wixstatic.com/media/b6a0a6_431d6337ed6d43a1b8a91d82a8cb7a1f~mv2.jpg"
      title="Hello there!"
      previewText="This is my first post!"
    />
    <PostPreview
      :is-admin="isAdmin"
      id="2"
      thumbnail="https://static.wixstatic.com/media/b6a0a6_431d6337ed6d43a1b8a91d82a8cb7a1f~mv2.jpg"
      title="Second post"
      previewText="This is my first post!"
    />
    <PostPreview
      :is-admin="isAdmin"
      id="3"
      thumbnail="https://static.wixstatic.com/media/b6a0a6_431d6337ed6d43a1b8a91d82a8cb7a1f~mv2.jpg"
      title="Third post"
      previewText="This is my first post!"
    />
  </section>
</template>

<script>
  import PostPreview from '@/components/Posts/PostPreview';

  export default {
    components: {
      PostPreview
    },
    props: {
      isAdmin: {
        type: Boolean,
        default: false
      }
    }
  };
</script>

<style lang="css">
  .featured-posts {
    display: flex;
    padding: 20px;
    box-sizing: border-box;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
  }
</style>
