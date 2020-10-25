<template>
  <div class="home">
    <div class="row home-row">
      <div class="col-md-6 col-one">
        <p class="title">
          Let Put An End to Police Brutality
        </p>

        <p>
          Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's
          standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to
          make a type specimen book.
        </p>

        <router-link to="/login"><a class="btn btn-primary">Get Started</a></router-link>
      </div>
      <div class="col-md-6 col-two">
        <img src="../assets/hand.png" />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
  import { defineComponent } from 'vue';

  export default defineComponent({
    name: 'Home',
    components: {},
  });
</script>

<style lang="scss" scoped>
  .home {
    height: 100vh;
  }

  .home-row {
    height: 100%;
  }
  .col-one {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 0 50px;
  }

  .col-two {
    display: flex;
    justify-content: center;

    img {
      height: 100%;
    }
  }

  .btn-primary {
    width: 150px;
  }

  .title {
    font-size: 5rem;
    font-weight: bold;
    line-height: 6rem;
  }
</style>
