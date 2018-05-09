<template>
  <div class="container">
    <nav class="navbar is-transparent">
      <div class="navbar-brand">
        <nuxt-link class="navbar-item" to="/" onclick="document.getElementById('sideBar').classList.toggle('is-active')">
          <h1 class="title has-text-primary">Sport</h1>
        </nuxt-link>
        <nuxt-link class="navbar-item" to="/search">
          <span class="icon has-text-primary">
            <i class="fas fa-lg fa-search"></i>
          </span>
        </nuxt-link>
        <nuxt-link class="navbar-item" to="/marks">
          <span class="icon has-text-primary">
            <i class="fas fa-lg fa-bookmark"></i>
          </span>
        </nuxt-link>
        <nuxt-link class="navbar-item" to="/notifications">
          <span class="icon has-text-primary">
            <i class="fas fa-lg fa-comment"></i>
          </span>
        </nuxt-link>
        <span id="nav-toggle" class="navbar-burger burger" onclick="document.getElementById('sideBar').classList.toggle('is-active')">
          <span></span>
          <span></span>
          <span></span>
        </span>
      </div>

      <div id="sideBar" class="navbar-menu">
        <div class="navbar-start">
          <nuxt-link class="navbar-item" to="/profile" onclick="document.getElementById('sideBar').classList.toggle('is-active')">
            <span class="icon has-text-primary">
              <i class="fas fa-user"></i>
            </span>
            Профиль
          </nuxt-link>
          <nuxt-link class="navbar-item" to="/chat" onclick="document.getElementById('sideBar').classList.toggle('is-active')">
            <span class="icon has-text-primary">
              <i class="fas fa-comment"></i>
            </span>
            Сообщения
          </nuxt-link>
          <nuxt-link class="navbar-item" to="/settings" onclick="document.getElementById('sideBar').classList.toggle('is-active')">
            <span class="icon has-text-primary">
              <i class="fas fa-cogs"></i>
            </span>
            Настройки
          </nuxt-link>
          <nuxt-link class="navbar-item" to="/help" onclick="document.getElementById('sideBar').classList.toggle('is-active')">
            <span class="icon has-text-primary">
              <i class="fas fa-question"></i>
            </span>
            Помощь
          </nuxt-link>
          <nuxt-link class="navbar-item" to="/becometrainer" onclick="document.getElementById('sideBar').classList.toggle('is-active')">
            <span class="icon has-text-primary">
              <i class="fas fa-question"></i>
            </span>
            Вы являетесь тренером
          </nuxt-link>
          <nuxt-link class="navbar-item" to="/createschool" onclick="document.getElementById('sideBar').classList.toggle('is-active')">
            <span class="icon has-text-primary">
              <i class="fas fa-home"></i>
            </span>
            У вас школа или клуб
          </nuxt-link>
          <nuxt-link class="navbar-item" to="/" onclick="document.getElementById('sideBar').classList.toggle('is-active')">
            <span class="icon has-text-primary">
              <i class="fas fa-sign-out-alt"></i>
            </span>
            Выйти
          </nuxt-link>
        </div>

        <div class="navbar-end">
          <div class="navbar-item">
            <div class="field is-grouped">
              <p class="control">
                <a class="bd-tw-button button" data-social-network="Twitter" data-social-action="tweet" data-social-target="http://localhost:4000" target="_blank" href="https://twitter.com/intent/tweet?text=Bulma: a modern CSS framework based on Flexbox&amp;hashtags=bulmaio&amp;url=http://localhost:4000&amp;via=jgthms">
                  <span class="icon">
                    <i class="fab fa-map-marker"></i>
                  </span>
                  <span>Мои места</span>
                </a>
              </p>
              <p class="control">
                <a class="button is-primary">
                  <span class="icon">
                    <i class="fas fa-calendar-alt"></i>
                  </span>
                  <span>Мои события</span>
                </a>
              </p>
            </div>
          </div>
        </div>
      </div>
</nav>
  </div>
</template>

<script>

    export default {
        name: "Navbar.vue"
    }
</script>

<style scoped>

</style>
