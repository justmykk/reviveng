<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-md-4"></div>
      <div class="col-md-4">
        <div class="card">
          <form @submit.prevent="submitForm">
            <h2>Revive NG</h2>
            <div class="form-group">
              <label for="exampleInputEmail1">Email address</label>
              <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" />
            </div>
            <div class="form-group">
              <label for="exampleInputPassword1">Password</label>
              <input type="password" class="form-control" id="exampleInputPassword1" />
            </div>
            <div class="form-group">
              <router-link to="/forgot-password"
                ><small id="emailHelp" class="form-text text-muted">Forgot Password?</small></router-link
              >
            </div>
            <button type="submit" class="btn btn-primary">Submit</button>

            <router-link to="/register"><a>Not Registered? Sign Up</a></router-link>
          </form>
        </div>
      </div>
      <div class="col-md-4"></div>
    </div>
  </div>
</template>

<script lang="ts">
  import { defineComponent } from 'vue';

  export default defineComponent({
    name: 'Login',
    methods: {
      submitForm() {
        this.$router.push('/projects');
      },
    },
  });
</script>

<style scoped lang="scss">
  .card {
    padding: 50px;
    margin-top: 50px;
  }

  h2 {
    text-align: center;
  }
</style>
