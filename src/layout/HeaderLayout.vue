<template>
  <div>
    <header class="py-3 mb-4 border-bottom">
      <div class="d-flex align-items-center">
        <a href="/" class="logo ">
          <router-link to="/">
            <img src="../assets/logo.jpeg" class="bi me-2" height="100" />
          </router-link>
        </a>
        </div>
    </header>
    <nav class="menu">
      <div class="d-flex flex-wrap">
        <ul class="nav me-auto">
          <li class="nav-item">
            <router-link to="/">
              <a href="#" class="nav-link px-2 active" aria-current="page"
                >Acceuil</a
              ></router-link
            >
          </li>
          <li class="nav-item">
            <router-link to="/constats"
              ><a href="#" class="nav-link px-2">Constats</a></router-link
            >
          </li>
          <li class="nav-item">
            <a href="#" class="nav-link px-2">Statistiques</a>
          </li>
        </ul>
        <ul class="nav">
          <li class="nav-item">
            <a href="#" class="nav-link px-2">Se connecter</a>
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped lang="scss">
.logo {
  margin: auto;
}
.menu {
  // py-2 bg-body-tertiary border-bottom

  background-color: rgba(38, 160, 204, $alpha: 1);
  padding-top: 2px;
  padding-bottom: 2px;
  color: white;
}
a {
  color: white;
  font-size: medium;
  font-weight: 600;
}
</style>
