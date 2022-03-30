<template>
  <section class="combiDeco">
    <h1 class="tituDeco">Selección de Decoraciónes</h1>
    <div class="decoContainer">
      <div class="decoSelection">
        <img src="../assets/bodacake.jpg" alt="" />
        <h3>Boda</h3>
        <label class="checkboxDeco">
          <input type="checkbox" id="boda" value="Boda" v-model="decoNames" />
          <span><i class="fas fa-check on"></i></span>
          <label for="boda"></label>
        </label>
      </div>

      <div class="decoSelection">
        <img src="../assets/cupcake.jpg" alt="" />
        <h3>Cupcake</h3>
        <label class="checkboxDeco">
          <input
            type="checkbox"
            id="cupcake"
            value="Cupcake"
            v-model="decoNames"
          />
          <span><i class="fas fa-check on"></i></span>
          <label for="cupcake"></label>
        </label>
      </div>

      <div class="decoSelection">
        <img src="../assets/halloweencake.jpg" alt="" />
        <h3>Festividad</h3>
        <label class="checkboxDeco">
          <input
            type="checkbox"
            id="festividad"
            value="Festividad"
            v-model="decoNames"
          />
          <span><i class="fas fa-check on"></i></span>
          <label for="festividad"></label>
        </label>
      </div>

      <br />
    </div>
    <div class="decoContainer">
      <div class="decoSelection">
        <img src="../assets/birthdaycake.jpg" alt="" />
        <h3>Cumpleaños</h3>
        <label class="checkboxDeco">
          <input
            type="checkbox"
            id="cumpleaños"
            value="Cumpleaños"
            v-model="decoNames"
          />
          <span><i class="fas fa-check on"></i></span>
          <label for="cumpleaños"></label>
        </label>
      </div>

      <div class="decoSelection">
        <img src="../assets/graducake.jpg" alt="" />
        <h3>Ocaciones especiales</h3>
        <label class="checkboxDeco">
          <input
            type="checkbox"
            id="ocaciones especiales"
            value="Ocaciones especiales"
            v-model="decoNames"
          />
          <span><i class="fas fa-check on"></i></span>
          <label for="ocaciones especiales"></label>
        </label>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data: () => ({
    decoNames: [],
  }),
};
</script>

<style lang="scss">
.tituDeco {
  color: #642a73;
  font-size: 30px;
  text-align: center;
  margin-bottom: 30px;
}

.combiDeco {
  background: #fff;
  margin-top: 80px;
}

.decoContainer {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
}

.decoContainer h3 {
  color: #642a73;
  font-size: 20px;
  text-align: center;
  margin-top: 5px;
  margin-bottom: 5px;
}

.decoSelection {
  text-align: center;
  width: 300px;
  height: 300px;
  margin-top: 50px;
  margin-bottom: 50px;
  overflow: unset;
  position: relative;
  box-shadow: 0 0 6px 0 rgba(0, 0, 0, 0.5);
}

.decoSelection > img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.checkboxDeco input:checked ~ span::after {
  background: rgba(9, 112, 9, 0.666);
  transform: scale(0.85) translate(35px);
}
.checkboxDeco input:checked ~ span .on {
  transform: translate(30px);
  opacity: 1;
}

.checkboxDeco input:checked ~ span .off {
  transform: translate(30px);
  opacity: 0;
}

.checkboxDeco input {
  display: none;
}

.checkboxDeco span {
  display: inline-block;
  width: 60px;
  height: 30px;
  border-radius: 30px;
  background: rgba(182, 26, 196, 0.254);
  cursor: pointer;
  box-shadow: inset 0px 0px 2px rgb(15, 15, 15);

  position: relative;
}

.checkboxDeco span::after {
  content: "";
  display: block;
  width: 30px;
  height: 30px;
  transform: scale(0.85);
  border-radius: 30px;
  background: rgba(163, 17, 17, 0.549);
  transition: 0.5s;
  box-shadow: inset 0px 0px 2px rgb(37, 37, 37);
}

.checkboxDeco i {
  position: absolute;
  left: 7px;
  top: 7px;
  z-index: 1;
  color: white;
  transition: 0.5s;
}

.checkboxDeco .on {
  opacity: 0;
  left: 7px;
  top: 7px;
}

.checkboxDeco .off {
  left: 9px;
  top: 7px;
}
</style>