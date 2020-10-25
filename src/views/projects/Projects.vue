<template>
  <div class="projects">
    <div class="container-fluid">
      <div class="row experience">
        <div class="col-md-6">
          <h2>Experiences / Projects</h2>
        </div>
        <div class="col-md-6 add-btn">
          <button class="btn btn-primary">Share Experience/Project</button>
        </div>
      </div>

      <div class="row">
        <div class="col-md-3" v-for="item in list" :key="item">
          <img src="../../assets/protest.png" alt="protest" class="item-image" />
          <p class="title">Lekki Massacre</p>
          <p class="time">October 20, 2020 7:00pm</p>
          <p class="content">
            There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in
            some form, by injected humour, or randomised words which don't look even slightly believable....
          </p>

          <a class="read-more">Read More</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
  import { defineComponent } from 'vue';

  export default defineComponent({
    name: 'Projects',
    data() {
      return {
        list: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
      };
    },
  });
</script>

<style lang="scss" scoped>
  .item-image {
    width: 100%;
  }
  .title {
    font-size: 1.4rem;
    font-weight: bold;
  }

  .time,
  .content {
    font-size: 0.8rem;
  }

  .time {
    margin: 5px 0;
  }

  .content {
    margin-bottom: 15px;
  }

  .read-more {
    font-weight: bold;
    font-size: 0.9rem;
  }

  .col-md-3 {
    margin-bottom: 50px;
  }

  .projects {
    padding: 50px 100px;
  }

  .add-btn {
    display: flex;
    justify-content: flex-end;
  }

  .experience {
      margin-bottom: 30px;

      h2 {
          font-weight: bold;
      }
  }
</style>
