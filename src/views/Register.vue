<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-md-4"></div>
      <div class="col-md-4">
        <div class="card">
          <form>
            <h2>Revive NG</h2>
            <div class="form-group">
              <label for="name">Name</label>
              <input type="text" class="form-control" id="name" aria-describedby="nameHelp" />
            </div>
            <div class="form-group">
              <label for="location">Location</label>
              <input class="form-control" id="location" aria-describedby="locationHelp" />
            </div>
            <div class="form-group">
              <label for="exampleInputEmail1">Email address</label>
              <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" />
            </div>
            <div class="form-group">
              <label for="exampleInputEmail1">Email address</label>
              <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" />
            </div>
            <div class="form-group">
              <label for="exampleInputPassword1">Password</label>
              <input type="password" class="form-control" id="exampleInputPassword1" />
            </div>
            <div class="form-group">
              <router-link to="/login"
                ><small class="form-text text-muted">Already registered? Login</small></router-link
              >
            </div>
            <button type="submit" class="btn btn-primary">Submit</button>
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
    name: 'Register',
  });
</script>

<style lang="scss" scoped>
  .card {
    padding: 50px;
    margin-top: 50px;
  }

  h2 {
    text-align: center;
  }
</style>
