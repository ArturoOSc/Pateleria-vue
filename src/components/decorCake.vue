<template>
  <section class="portafolio2" id="menu">
    <div class="contenedor2">
      <h2 class="titulo2">Decoraciónes</h2>
      <div class="galeria-port2">
        <div class="imagen-port2">
          <img src="../assets/bodacake.jpg" alt="" />
          <div class="hover-galeria2">
            <a href="pedido.html"
              ><img src="../assets/bolsa-de-la-compra.png" alt=""
            /></a>
            <p>Boda</p>
            <p>$1200</p>
          </div>
        </div>
        <div class="imagen-port2">
          <img src="../assets/cupcake.jpg" alt="" />
          <div class="hover-galeria2">
            <a href="pedido.html"
              ><img src="../assets/bolsa-de-la-compra.png" alt=""
            /></a>
            <p>Cupcake</p>
            <p>$600</p>
          </div>
        </div>
        <div class="imagen-port2">
          <img src="../assets/halloweencake.jpg" alt="" />
          <div class="hover-galeria2">
            <a href="pedido.html"
              ><img src="../assets/bolsa-de-la-compra.png" alt=""
            /></a>
            <p>Festividades</p>
            <p>$700</p>
          </div>
        </div>
        <div class="imagen-port2">
          <img src="../assets/birthdaycake.jpg" alt="" />
          <div class="hover-galeria2">
            <a href="pedido.html"
              ><img src="../assets/bolsa-de-la-compra.png" alt=""
            /></a>
            <p>Cumpleaños</p>
            <p>$350</p>
          </div>
        </div>
        <div class="imagen-port2">
          <img src="../assets/graducake.jpg" alt="" />
          <div class="hover-galeria2">
            <a href="pedido.html"
              ><img src="../assets/bolsa-de-la-compra.png" alt=""
            /></a>
            <p>Ocaciones especiales</p>
            <p>$500</p>
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
.titulo2 {
  color: #b11b61ef;
  font-size: 30px;
  text-align: center;
  margin-bottom: 30px;
}
.portafolio2 {
  background: #f2f2f2;
  margin-top: 80px;

}
.galeria-port2 {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
}

.imagen-port2 {
  width: 15%;
  height: auto;
  margin-bottom: 10px;
  overflow: hidden;
  position: relative;
  cursor: pointer;
  box-shadow: 0 0 6px 0 rgba(0, 0, 0, 0.5);
}

.imagen-port2 > img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.hover-galeria2 {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  transform: scale(0);
  background: hsla(322, 78%, 48%, 0.7);
  transition: transform 0.5s;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.hover-galeria2 img {
  width: 50px;
}

.hover-galeria2 p {
  color: #fff;
}

.imagen-port2:hover .hover-galeria2 {
  transform: scale(1);
}
</style>
