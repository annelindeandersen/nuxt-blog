<template>
  <div class="single-post-page">
    <section class="post">
      <h1>Title of post</h1>
      <div class="post-details">
        <div>Last updated on xxx</div>
        <div>Written by name</div>
      </div>
      <hr />
      <p>Content of post</p>
    </section>
    <section class="post-feedback">
      <p>
        What do you think about the post? mail to
        <a href="mailto:anne_linde@yahoo.dk">this email address</a>
      </p>
    </section>
  </div>
</template>

<style lang="css" scoped>
.single-post-page {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 20px;
  width: 100vw;
  /* height: 100vh; */
}

.post {
  background: rgba(128, 128, 128, 0.166);
  padding: 20px;
  width: 50%;
}
</style>
