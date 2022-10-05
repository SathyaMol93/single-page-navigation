<template>
  <div class="main">
    <div class="nav">
      <h1 class="logo">Demo</h1>
      <ul class="nav-items">
        <li class="item">
          <nuxt-link :to="'#anchor-1'"> Anchor 1 </nuxt-link>
        </li>
        <li class="item">
          <nuxt-link :to="'#anchor-2'"> Anchor 2 </nuxt-link>
        </li>
      </ul>
    </div>
    <div id="anchor-1" class="anchor-1"></div>
    <div id="anchor-2" class="anchor-2"></div>
  </div>
</template>
<script setup></script>
<style>
.main {
  width: 100%;
  height: 100%;
}
.nav {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  background: #c0c0c0;
  padding: 0px 10px;
  align-items: center;
  position: sticky;
  top: 0;
  height: 80px;
}
.logo {
  font-weight: bold;
  font-size: 1.5rem;
}
.nav-items {
  display: flex;
  flex-direction: row;
  align-items: center;
  list-style-type: none;
  height: 100%;
}

.nav-items .item {
  font-weight: bold;
  font-size: 1.2rem;
}

.nav-items .item a {
  text-decoration: none !important;
  color: #000000;
}

.item:not(:first-child) {
  margin-left: 10px;
  padding: 0 10px;
  border-left: solid 2px;
}

.anchor-1 {
  background: #ffcce5;
  width: 100%;
  height: 100vh;
  margin-top: -80px;
  padding-top: 80px;
}

.anchor-2 {
  background: #ccffff;
  width: 100%;
  height: 100vh;
  margin-top: -80px;
  padding-top: 80px;
}
</style>
