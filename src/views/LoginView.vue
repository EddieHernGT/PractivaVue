<template>
  <main class="main">
    <h1>Roma</h1>
    <form class="inicio" action="pastelero.html">
      <label for="email">Correo:</label>
      <input id="email" type="email" name="correo">
      <label for="pass">Contraseña:</label>
      <input id="pass" type="password">
      <router-link to="/home_pastelero"><input type="submit"></router-link>
    </form>
  </main>
</template>

<style>
.inicio{
  align-content: center;
  max-width: 20%;
  margin: 20% 40%;
  display: grid;
  grid-template-columns: repeat(2,1fr);
}
.inicio input{
  grid-column: 2;
}
</style>