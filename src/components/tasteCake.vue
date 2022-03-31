<template>
  <section class="portafolio" id="menu">
    <div class="contenedor">
      <h2 class="titulo">Menú</h2>
      <div class="galeria-port">
        <div class="imagen-port">
          <img src="../assets/chocolate.jpg" alt="" />
          <h2>chocolate</h2>
          <div class="hover-galeria">
            <a href="pedido.html"
              ><img src="../assets/bolsa-de-la-compra.png" alt=""
            /></a>
            <p>Chocolate</p>
            <p>$300</p>
          </div>
        </div>
        <div class="imagen-port">
          <img src="../assets/fresa.jpg" alt="" />
          <div class="hover-galeria">
            <a href="pedido.html"
              ><img src="../assets/bolsa-de-la-compra.png" alt=""
            /></a>
            <p>Fresa</p>
            <p>$400</p>
          </div>
        </div>
        <div class="imagen-port">
          <img src="../assets/cajeta.jpg" alt="" />
          <div class="hover-galeria">
            <a href="pedido.html"
              ><img src="../assets/bolsa-de-la-compra.png" alt=""
            /></a>
            <p>Cajeta</p>
            <p>$300</p>
          </div>
        </div>
        <div class="imagen-port">
          <img src="../assets/moras.jpg" alt="" />
          <div class="hover-galeria">
            <a href="pedido.html"
              ><img src="../assets/bolsa-de-la-compra.png" alt=""
            /></a>
            <p>Moras</p>
            <p>$350</p>
          </div>
        </div>
        <div class="imagen-port">
          <img src="../assets/oreo.jpg" alt="" />
          <div class="hover-galeria">
            <a href="pedido.html"
              ><img src="../assets/bolsa-de-la-compra.png" alt=""
            /></a>
            <p>Oreo</p>
            <p>$400</p>
          </div>
        </div>
        <div class="imagen-port">
          <img src="../assets/red-velvet.jpg" alt="" />
          <div class="hover-galeria">
            <a href="pedido.html"
              ><img src="../assets/bolsa-de-la-compra.png" alt=""
            /></a>
            <p>Red velvet</p>
            <p>$450</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss">
.titulo {
  color: #642a73;
  font-size: 30px;
  text-align: center;
  margin-bottom: 30px;
}
.portafolio {
  background: #f2f2f2;
  margin-top: 80px;
}
.galeria-port {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
}

.imagen-port {
  width: 15%;
  height: auto;
  margin-bottom: 10px;
  overflow: hidden;
  position: relative;
  cursor: pointer;
  box-shadow: 0 0 6px 0 rgba(0, 0, 0, 0.5);
}

.imagen-port > img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.hover-galeria {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  transform: scale(0);
  background: hsla(273, 91%, 27%, 0.7);
  transition: transform 0.5s;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.hover-galeria img {
  width: 50px;
}

.hover-galeria p {
  color: #fff;
}

.imagen-port:hover .hover-galeria {
  transform: scale(1);
}
</style>
