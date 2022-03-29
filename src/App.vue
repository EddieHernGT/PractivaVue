<template>
  <header>
    <div class="barra">
      <router-link to="/"><img src="./assets/logo.jpg"></router-link>
      <nav ><ul class="menu">
        <li><a href="/#nuestrosProd">Productos</a></li>
        <li><a href="/#pedidos">Pedidos</a></li>
        <li><a href="/#ubi">Sucursal</a></li>
        <li><router-link to="/login">Ingresa</router-link></li>
      </ul></nav>
    </div>
  </header>
  <router-view/>
  <footer>
    <div>
      <h4>Links</h4>
      <nav ><ul  class="nav">
        <li><a href="/#nuestrosProd">Productos</a></li>
        <li><a href="/#pedidos">Pedidos</a></li>
        <li><a href="/#ubi">Sucursal</a></li>
      </ul></nav>
    </div>
    <div class="descrip">
      <h4>Roma</h4>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque non sagittis nunc.</p>
    </div>
    <div class="contacto">
      <h4>Contacto</h4>
      <ul>
        <li><i class="fa-solid fa-envelope"></i> roma_pasteleria@gmial.com</li>
        <li><i class="fa-solid fa-location-dot"></i> Avenida del paraiso #420</li>
        <li><i class="fa-solid fa-phone"></i> +525544332211</li>
      </ul>
    </div>
  </footer>
</template>

<style>
html{
  background-color: #ffbaba;
}
/* Chrome, Safari, Edge, Opera */
input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button {
  -webkit-appearance: none;
  margin: 0;
}

/* Firefox */
input[type=number] {
  -moz-appearance: textfield;
}
body{
  margin: 0;
}
main{
  margin: 0 50px;
  background-color: white;
  justify-content: center;
}
h2{
  font-weight: bold;
  font-size: x-large;
  margin: 30px 0;
  text-align: center;
}
ul{
  list-style-type: none;
}
img{
  max-width: 70%;
}
.barra{
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 10px 50px;
  max-height: 50px;
  border: 3px white solid;
}
.barra img{
  margin: 0 30px;
  max-width: 5%;
  min-width: 5%;
}

.menu{
  display: flex;
  flex-direction: row;
  align-items: center;
}
.menu li a{
  color: #494848;
  text-decoration: none;
  padding:10px;
}
.menu li a:hover{
  color:black;
  background-size: contain;
  background-color: white;
}
.menu li router-link{
  cursor: pointer;
  color: #494848;
  text-decoration: none;
  padding:0;
}
.menu li router-link:hover{
  color:black;
  background-color: white;
}
footer{
  background: #d49898;
  margin-top: 20px;
  padding-top: 5%;
  padding-right: 10%;
  padding-left: 10%;
  padding-bottom: 5%;
  display: grid;
  grid-template-columns: repeat(3,1fr);
}
.nav{
  display: flex;
  flex-direction: column;
  align-content: space-around;
}
.nav a{
  text-decoration: none;
  color: #494848;
}
.nav a:hover{
  color: white;
}
.main{
  min-height: 80vh;
}
.main h1{
  text-align: center;
  background: #d49898;
}
.pastel{
  justify-content: center;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-auto-rows: minmax(30px, auto);
}
.pastel .titulo{
  grid-row: 1;
  grid-column: 1 / 4;
  max-height: fit-content;
}
.pastel .uno{
  grid-row: 2;
  grid-column: 1;
}
.pastel .dos{
  grid-row: 2;
  grid-column: 2;
}
.pastel .tres{
  grid-row: 2;
  grid-column: 3;
}
.elemento{
  padding: 20px 0px;
  border-style: dotted;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>
