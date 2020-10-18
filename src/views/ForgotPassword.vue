<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-md-4"></div>
      <div class="col-md-4">
        <div class="card">
          <form>
            <h2>Revive NG</h2>
            <div class="form-group">
              <label for="exampleInputEmail1">Email address</label>
              <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" />
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
    name: 'ForgotPassword',
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
