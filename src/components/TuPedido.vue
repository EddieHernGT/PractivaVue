<template>
  <h2 id="pedidos">Arma tu pastel</h2>
  <div class="orden">
    <img src="../assets/pastel.jpg">
    <form id="orden">
      <h3>Datos</h3>
      <label for="name">Nombre:</label>
      <input id="name" type="text" name="nombre">
      <label for="email">Correo:</label>
      <input id="email" type="email" name="correo">
      <label for="phone">No. Telefono:</label>
      <input id="phone" type="number" minlength="10" name="telefono">
      <h3>Sabores</h3>
      <div>
        <label><input type="checkbox" id="flavor1" value="fresa"> Fresa</label>
        <label><input type="checkbox" id="flavor2" value="Chocolate"> Chocolate</label>
        <label><input type="checkbox" id="flavor3" value="Vainilla"> Vainilla</label>
      </div>
      <h3>Adornos</h3>
      <div>
        <label><input type="checkbox" id="deco1" value="chispas"> Chispas</label>
        <label><input type="checkbox" id="deco2" value="letrero"> Letrero</label>
        <label><input type="checkbox" id="deco3" value="flores"> Chispas</label>
      </div>
      <h3>Detalles</h3>
      <textarea name="comment" form="orden">Enter text here...</textarea>
      <input type="submit">
    </form>
  </div>
</template>

<script>
export default {
  name: "TuPedido"
}
</script>

<style scoped>
.orden{
  display: flex;
  flex-direction: row;
  flex-flow: wrap;
  justify-content: space-evenly;
}
.orden img{
  max-width: 50%;
}
.orden form{
  padding: 30px;
  display: grid;
  grid-auto-rows: minmax(30px, auto);
  grid-template-columns: repeat(2,1fr);
  align-items: center;
}
.orden form h3{
  grid-column: 1/3;
}
.orden form label{
  grid-column: 1;
  text-align: right;
  margin-right: 20px;
}
.orden form input{
  grid-column: 2;
}
.orden form div{
  grid-column: 1/3;
  display: flex;
  justify-content: center;
}
.orden form textarea{
  min-height: 60px;
  grid-column: 1/3;
}
</style>