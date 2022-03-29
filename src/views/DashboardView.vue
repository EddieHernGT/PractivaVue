<template>
  <main class="main pastelero">
    <h1>Bienvenido</h1>
    <div class="productosDisp">
      <h2>Productos disponibles</h2>
      <ul class="pastel dispo">
        <li class="titulo"><h3>Sabores</h3></li>
        <li class="elemento uno"><img src="../assets/fresa.jpg"><p>Fresa</p><p>Cantidad restante:</p></li>
        <li class="elemento dos"><img src="../assets/chocolate.jpg"><p>Chocolate</p><p>Cantidad restante:</p></li>
        <li class="elemento tres"><img src="../assets/vainilla.jpg"><p>Vainilla</p><p>Cantidad restante:</p></li>
      </ul>
      <ul class="pastel dispo">
        <li class="titulo"><h3>Adornos</h3></li>
        <li class="elemento uno"><img src="../assets/Chispas.jpg"><p>Chispas</p><p>Cantidad restante:</p></li>
        <li class="elemento dos"><img src="../assets/letrero.png"><p>Letrero "Felicidades"</p><p>Cantidad restante:</p></li>
        <li class="elemento tres"><img src="../assets/flores.jpg"><p>Flores</p><p>Cantidad restante:</p></li>
      </ul>
    </div>
    <div class="nuevasOrdenes">
      <h2>Nuevas Ordenes</h2>
      <ul>
        <li>Orden 1<ul>
          <li>Nombre:</li>
          <li>Sabor:</li>
          <li>Adornos:</li>
          <li>Descripcion:</li>
          <li>Subtotal:</li>
        </ul></li>
        <li>Orden 1<ul>
          <li>Nombre:</li>
          <li>Sabor:</li>
          <li>Adornos:</li>
          <li>Descripcion:</li>
          <li>Subtotal:</li>
        </ul></li>
      </ul>
    </div>
  </main>
</template>

<script>
export default {
  name: "DashboardView"
}
</script>

<style scoped>
.productosDisp{
  max-width: 100%;
  padding-bottom: 5%;
}
.pastelero{
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}
.pastelero h1{
  grid-column: 1/3;
}
.pastelero.nuevasOrdenes{
  text-align: center;
}
</style>