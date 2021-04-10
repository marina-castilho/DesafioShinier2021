<template>
  <!-- <div class="container is-widescreen"> -->
  <!-- <b-navbar>
      <template #brand>
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <img
            src="../assets/pictures/logo_an 1.svg"
            alt="Logo Analytis"
            ratio="16by9"
          />
          <b-input
            placeholder="Buscar Funcionalidade"
            type="search"
            icon="magnify"
            icon-clickable
            @icon-click="searchIconClick"
          />
        </b-navbar-item>
      </template>

      <template #end>
        <img
          src="../assets/pictures/Rectangle.svg"
          alt="Logo Analytis"
          ratio="16by9"
        />
        <section class="hero is-small">
          <div class="hero-body">
            <p class="title">Super Admin</p>
            <p class="subtitle">SUPER ADMIN</p>
          </div>
        </section>
      </template>
    </b-navbar> -->
  <div class="container is-widescreen">
    <b-navbar :fixed-top="true">
      <template #brand>
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <img
            src="../assets/pictures/logo_an 1.svg"
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
        <img
          src="../assets/pictures/Rectangle.svg"
          alt="Logo Analytis"
          ratio="16by9"
        />
        <section class="hero is-small">
          <div class="hero-body">
            <p class="title">Super Admin</p>
            <p class="subtitle">SUPER ADMIN</p>
          </div>
        </section>
      </template>
    </b-navbar>

    <b-menu>
      <b-menu-list label="Menu">
        <b-menu-item class="menu-item" :active="isActive" expanded>
          <template>
            <img src="pictures/dash.svg" class="icon is-small" />
            Dashboard
          </template>
        </b-menu-item>
        <!-- <b-menu-item class="menu-item">
          <img src="src/assets/pictures/grupos.svg" alt="Analitcs" />
          Grupos
        </b-menu-item>
        <b-menu-item class="menu-item">
          <img src="src/assets/pictures/users.svg" alt="Analitcs" />
          Usuários
        </b-menu-item>
        <b-menu-item class="menu-item">
          <img src="src/assets/pictures/sistemas.png" alt="Analitcs" />
          Sistemas
        </b-menu-item>
        <b-menu-item class="menu-item">
          <img src="src/assets/pictures/categ.svg" alt="Analitcs" />
          Categorias
        </b-menu-item> -->

        <!-- <b-menu-item icon="information-outline" label="Info"></b-menu-item>
        <b-menu-item icon="settings" :active="isActive" expanded>
          <template #label="props">
            Administrator
            <b-icon
              class="is-pulled-right"
              :icon="props.expanded ? 'menu-down' : 'menu-up'"
            ></b-icon>
          </template>
          <b-menu-item icon="account" label="Users"></b-menu-item>
          <b-menu-item icon="cellphone-link">
            <template #label>
              Devices
              <b-dropdown
                aria-role="list"
                class="is-pulled-right"
                position="is-bottom-left"
              >
                <template #trigger>
                  <b-icon icon="dots-vertical"></b-icon>
                </template>
                <b-dropdown-item aria-role="listitem">Action</b-dropdown-item>
                <b-dropdown-item aria-role="listitem"
                  >Another action</b-dropdown-item
                >
                <b-dropdown-item aria-role="listitem"
                  >Something else</b-dropdown-item
                >
              </b-dropdown>
            </template>
          </b-menu-item>
          <b-menu-item
            icon="cash-multiple"
            label="Payments"
            disabled
          ></b-menu-item>
        </b-menu-item>
        <b-menu-item icon="account" label="My Account">
          <b-menu-item label="Account data"></b-menu-item>
          <b-menu-item label="Addresses"></b-menu-item>
        </b-menu-item>
      </b-menu-list>
      <b-menu-list>
        <b-menu-item
          label="Expo"
          icon="link"
          tag="router-link"
          target="_blank"
          to="/expo"
        ></b-menu-item>
      </b-menu-list>
      <b-menu-list label="Actions">
        <b-menu-item label="Logout"></b-menu-item>
      </b-menu-list> -->
      </b-menu-list>
    </b-menu>
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
