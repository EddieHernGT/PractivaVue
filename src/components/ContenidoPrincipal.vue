<template>
  <div class="parallax">
    <div>
      <h1>Roma</h1>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer egestas congue ante,
        quis ultricies turpis egestas a. Mauris dignissim nunc quis lectus pellentesque ultricies.
        Donec efficitur velit dapibus massa egestas, eget ornare odio pretium.
        Suspendisse potenti. Quisque placerat erat eget fermentum ultricies.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContenidoPrincipal"
}
</script>

<style scoped>
.parallax {
  background-image: url("../assets/header.jpg");
  max-height: 500px;
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.parallax div{
  font-weight: bold;
  font-size: x-large;
  color: black;
  text-align: center;
  justify-content: center;
  padding: 10%;
}
</style>