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
          <div class="barra">
            <b-input
              placeholder="Buscar Funcionalidade"
              type="search"
              icon="magnify"
              icon-clickable
              @icon-click="searchIconClick"
              custom-class="input"
            />
            <p class="acesso">Cadastrar novo usuário</p>
          </div>
        </b-navbar-item>
      </template>

      <template #end>
        <div class="admin">
          <div class="retangulo">
            <img
              src="pictures/Rectangle.svg"
              alt="Logo Analytis"
              ratio="16by9"
            />
          </div>
          <section class="title">
            <div class="title-body">
              <p class="title is-5">Super Admin</p>
              <p class="subtitle is-6">SUPER ADMIN</p>
            </div>
          </section>
        </div>
      </template>
    </b-navbar>
    <div class="botao">
      <b-button type="is-success">Salvar</b-button>
    </div>
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
</style>
