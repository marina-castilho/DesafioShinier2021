<template>
  <b-navbar>
    <template #brand>
      <b-navbar-item tag="router-link" :to="{ path: '/' }">
        <img
          src="../assets/pictures/logo_an 1.svg"
          alt="Logo Analytis"
          class="icon is-large"
        />
      </b-navbar-item>
    </template>
    <template #start>
      <b-navbar-item href="#"> Home </b-navbar-item>
      <b-navbar-item href="#"> Documentation </b-navbar-item>
      <b-navbar-dropdown label="Info">
        <b-navbar-item href="#"> About </b-navbar-item>
        <b-navbar-item href="#"> Contact </b-navbar-item>
      </b-navbar-dropdown>
    </template>

    <template #end>
      <b-navbar-item tag="div">
        <div class="buttons">
          <a class="button is-primary">
            <strong>Sign up</strong>
          </a>
          <a class="button is-light"> Log in </a>
        </div>
      </b-navbar-item>
    </template>
  </b-navbar>
</template>


        
<script>
export default {
  data() {
    return {
      isActive: true,
    };
  },
};
</script>
<script>
export default {
  name: "Usuários",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
</style>
