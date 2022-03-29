<template>
  <main>
    <ContenidoPrincipal></ContenidoPrincipal>
  </main>
  <section class="productos">
    <NuestrosProductos></NuestrosProductos>
  </section>
  <section class="productos">
    <TuPedido></TuPedido>
  </section>
  <section class="productos">
    <NuestraTienda></NuestraTienda>
  </section>
</template>

<script>
// @ is an alias to /src
import ContenidoPrincipal from '../components/ContenidoPrincipal';
import NuestrosProductos from '../components/NuestrosProductos';
import TuPedido from '../components/TuPedido';
import NuestraTienda from "../components/NuestraTienda";

export default {
  name: 'HomeView',
  components: {
    ContenidoPrincipal,
    NuestrosProductos,
    TuPedido,
    NuestraTienda
  }
}
</script>
<style>
.productos{
  margin: 0 50px;
  padding: 30px 70px;
  background-color: white;
}
.productos h2{
  background: #d49898;
  text-decoration: underline;
}
</style>