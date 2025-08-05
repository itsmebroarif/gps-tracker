<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-light bg-light shadow-sm mb-4">
      <div class="container">
        <router-link class="navbar-brand fw-bold" to="/"
          >GPS Dashboard</router-link
        >
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <router-link class="nav-link" to="/">Dashboard</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/about">About</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <main class="container">
      <router-view />
    </main>
  </div>
</template>

<style scoped>
body {
  zoom: 90%;
  margin: 0;
  font-family: "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  background-color: #f9f9f9;
}

.nav-link.router-link-exact-active {
  color: #0d6efd !important;
  font-weight: bold;
  border-bottom: 2px solid #0d6efd;
}
</style>
