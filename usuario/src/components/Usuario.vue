<template>
  <div class="container is-widescreen">
    <b-navbar :fixed-top="true">
      <template #brand>
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <img
            src="pictures/logo_an 1.svg"
            alt="Logo Analytis"
            ratio="16by9"
            class="logo"
          />
          <b-input
            placeholder="Buscar Funcionalidade"
            type="search"
            icon="magnify"
            icon-clickable
            @icon-click="searchIconClick"
            custom-class="input"
          />
        </b-navbar-item>
      </template>

      <template #end>
        <img src="pictures/Rectangle.svg" alt="Logo Analytis" ratio="16by9" />
        <section class="hero is-small">
          <div class="hero-body">
            <p class="title">Super Admin</p>
            <p class="subtitle">SUPER ADMIN</p>
          </div>
        </section>
      </template>
    </b-navbar>
    <div class="body">
      <b-menu>
        <b-menu-item class="menu-item" :active="isActive" expanded>
          <template>
            <img src="pictures/dash.svg" class="icon is-small" />
            Dashboard
          </template>
        </b-menu-item>
        <b-menu-item class="menu-item" :active="isActive" expanded>
          <template>
            <img src="pictures/grupos.svg" class="icon is-small" />
            Grupos
          </template>
        </b-menu-item>
        <b-menu-item class="menu-item" :active="isActive" expanded>
          <template>
            <img src="pictures/users.svg" class="icon is-small" />
            Usuários
          </template>
        </b-menu-item>
        <b-menu-item class="menu-item" :active="isActive" expanded>
          <template>
            <img src="pictures/sistemas.png" class="icon is-small" />
            Sistemas
          </template>
        </b-menu-item>
        <b-menu-item class="menu-item" :active="isActive" expanded>
          <template>
            <img src="pictures/categ.svg" class="icon is-small" />
            Categorias
          </template>
        </b-menu-item>
      </b-menu>
      <div class="content">
        <h1></h1>
        <div></div>
      </div>
    </div>
  </div>
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
nav.navbar.is-fixed-top {
  background: transparent;
}
</style>
