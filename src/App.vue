<template>
  <header>
    <nav>
      <a href="#inicio">Inicio</a>
      <a href="#about us">Productos</a>
      <a href="#menu">Menú</a>
      <a href="#clientes">Clientes</a>
      <a href="#servicio">Servicios</a>
      <a href="#footer">Contacto</a>
    </nav>
    <div class="textos-header">
      <h1>Pastelería</h1>
      <br><br>
      <h2>l'amour en une bouchée</h2>
    </div>
  </header>
  <br>
  <tasteCake />
  <decorCake />
  <combiTaste />
  <combiDeco />
  <infoCake />
</template>

<script>
import combiTaste from "@/components/combiTaste.vue"
import tasteCake from "@/components/tasteCake.vue" 
import decorCake from "@/components/decorCake.vue"
import combiDeco from "@/components/combiDeco.vue"
import infoCake from "@/components/infoCake.vue"
export default{
  name: "App",
  components:{
    combiTaste,
    tasteCake,
    decorCake,
    combiDeco,
    infoCake   
  }
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  scroll-behavior: smooth;
}

body {
  font-family: "open sans";
}

header {
  font-family: "open sans";
  background-image: url(../src/assets/Portada.jpg);
  background-size: 100%;
  background-position-x: center;
  background-repeat: no-repeat;
  padding: auto;
  margin: auto;
}

nav {
  text-align: right;
  padding: 30px 50px 0 0;
}

nav > a {
  color: #fff;
  font-weight: 300;
  text-decoration: none;
  margin-right: 10px;
}

nav > a:hover {
  text-decoration: underline;
}

header .textos-header {
  display: flex;
  height: 430px;
  width: 100%;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  text-align: center;
}

.textos-header h1 {
  font-size: 50px;
  color: #fff;
}

.textos-header h2 {
  font-size: 30px;
  font-weight: 300;
  color: #fff;
}
</style>
