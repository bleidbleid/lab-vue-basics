<template>
  <div class="section">
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <a>
          <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/01/SX3_logo.svg/1920px-SX3_logo.svg.png" width="85" height="42">
        </a>

        <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div id="navbarBasicExample" class="navbar-menu">
        <div class="navbar-start">
          <a class="navbar-item">
            Les Tres Bessones
          </a>

          <a class="navbar-item">
            Contes
          </a>

          <div class="navbar-item has-dropdown is-hoverable">
            <a class="navbar-link">
              Personatges
            </a>

            <div class="navbar-dropdown">
              <a class="navbar-item">
                Bessones
              </a>
              <a class="navbar-item">
                Ratolins
              </a>
              <a class="navbar-item">
                Bruixa i Mussol
              </a>
              <hr class="navbar-divider">
              <a class="navbar-item">
                Altres
              </a>
            </div>
          </div>
        </div>

        <div class="navbar-end">
          <div class="navbar-item">
            <div class="buttons">
              <button class="el-principal">
                <a>Sign up</a>
              </button>
              <button class="el-secundari">
                <a>Log in</a>
              </button>
            </div>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>
<script setup>
// import { ref } from 'vue';
</script>

<style scoped>
.el-principal {
  font-family: 'Patrick Hand SC', cursive;
  font-size: 1.2rem;
  padding: 4px 16px;
  background-color: #A56DA6;
}

.el-principal a {
  color: #F3EAE5;
}

.el-secundari {
  font-family: 'Patrick Hand SC', cursive;
  font-size: 1.2rem;
  padding: 4px 16px;
  border-color: #A56DA6;

}

.el-secundari a {
  color: #A56DA6;
}

.buttons {
  gap: 6px;
}
</style>