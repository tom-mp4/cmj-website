<script setup>

</script>

<template>
  <div class="landing">
    <div class="left">
      <h1 class="title">Nos Projets.</h1>
      <p class="description">
        Découvrez les projets, actions et idées que nous portons au CMJ.
      </p>
    </div>
    <div class="right">
      <img src="@/assets/image/project-illustration.png" alt="project-illustration" class="image">
    </div>
  </div>
</template>

<style scoped lang="scss">
@use '@/assets/styles/_colors.scss';
@use '@/assets/styles/_fonts.scss';

.landing {
  display: flex;
  align-items: center;
  padding: 14% 0;
  width: 70%;
  gap: 50px;

  .left {
    display: flex;
    flex-direction: column;
    gap: 25px;
    width: 50%;

    .title {
      font-family: fonts.$greycliff;
      color: colors.$black;
      font-size: 6rem;
      line-height: 1;
      letter-spacing: -0.06em;
    }

    .description {
      font-family: fonts.$montserrat;
      color: colors.$black;
      font-size: 1.2rem;
      line-height: 1;
    }
  }

  .right {
    display: flex;
    align-items: center;
    justify-content: center;

    .image {
      width: 95%;
    }
  }
}

@media (max-width: 576px) {
  .landing {
    flex-direction: column;
    padding: 50% 0;
    width: 80%;

    .left {
      align-items: center;
      justify-content: center;
      width: 100%;
      gap: 20px;

      .title {
        font-size: 4rem;
      }
    }

    .right {
      display: flex;
      align-items: center;
      justify-content: center;

      .image {
        width: 100%;
      }
    }
  }
}

</style>
