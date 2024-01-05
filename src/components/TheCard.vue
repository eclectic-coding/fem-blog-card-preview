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
  display: flex;
  width: 384px;
  flex-direction: column;
  align-items: flex-start;
  gap: 24px;
  flex-shrink: 0;
  border-radius: 20px;
  border: 1px solid var(--color-black);
  background: var(--color-card-background);
  box-shadow: 8px 8px 0 0 #000;

  @media (max-width: 375px) {
    width: 327px;
  }

  & > img {
    display: flex;
    align-items: center;
    align-self: stretch;
    border-radius: 10px;
  }

  &__content {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 12px;
    align-self: stretch;
    color: var(--color-text-grey);
  }

  &__button {
    display: flex;
    padding: 4px 12px;
    justify-content: center;
    align-items: center;
    gap: 8px;
    border-radius: 4px;
    background: var(--color-primary);

    color: var(--color-text-dark);
    font-size: 14px;
    font-weight: 800;
    line-height: 150%;
    width: 89px;
  }

  &__subtitle {
    color: var(--color-text-dark);

    font-family: Figtree,serif;
    font-size: 14px;
    font-style: normal;
    font-weight: 500;
    line-height: 150%; /* 21px */
  }

  h1 {
    color: var(--color-text-dark);
    font-family: Figtree,serif;
    font-size: 24px;
    font-style: normal;
    font-weight: 800;
    line-height: 150%; /* 36px */
    cursor: pointer;
    transition: color 0.2s ease-in-out;

    &:hover {
      color: var(--color-primary);
    }

    @media (max-width: 375px) {
      font-size: 20px;
    }
  }


  &__footer {
    color: var(--color-text-dark);
    font-weight: 800;
  }

}
</style>