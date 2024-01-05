<script setup>

</script>

<template>
  <div class="card p-4">
    <img src="../assets/images/illustration-article.svg" alt="">
    <div class="card__content">
      <div class="card__button">Learning</div>
      <p class="card__subtitle">Published
        <time datetime="2023-12-21">21 Dec 2023</time>
      </p>
      <h1>HTML & CSS foundations</h1>
      <div class="card__content">
        These languages are the backbone of every website, defining structure, content, and presentation.
      </div>
    </div>
    <div class="card__footer">
      <img src="../assets/images/image-avatar.webp" width="32" height="32" alt="" class="me-2">
      <span>Greg Hopper</span>
    </div>
  </div>
</template>

<style scoped lang="scss">
.card {
  width: 384px;
  border-radius: 20px;
  border: 1px solid var(--color-black);
  background: var(--color-card-background);
  box-shadow: 8px 8px 0 0 #000;

  & > img {
    display: flex;
    align-items: center;
    align-self: stretch;
    border-radius: 10px;
  }

  &__content {
    color: var(--color-text-grey);
    padding: 1rem 0;
  }

  &__button {
    display: flex;
    padding: 4px 12px;
    margin: 0.75rem 0;
    justify-content: center;
    align-items: center;
    background: var(--color-primary);
    border-radius: 4px;
    color: var(--color-text-dark);
    font-size: 14px;
    font-weight: 800;
    line-height: 150%;
    width: 89px;
  }

  h1 {
    color: var(--color-text-dark);
    font-family: Figtree, serif;
    font-size: 24px;
    font-style: normal;
    font-weight: 800;
    line-height: 150%;
    cursor: pointer;
    transition: color 0.2s ease-in-out;

    &:hover {
      color: var(--color-primary);
    }
  }

  &__subtitle {
    color: var(--color-text-dark);
    font-size: 14px;
  }

  &__footer {
    color: var(--color-text-dark);
    font-weight: 800;
  }

}
</style>