<template>
  <section class="combi">
      <h1 class="tituCake">Selección de sabores</h1>
    <div class="cakeContainer">
      <div class="cakeSelection">
        <img src="../assets/chocolate.jpg" alt="" />
        <h3>Chocolate</h3>
        <label class="mycheckbox">
          <input
            type="checkbox"
            id="chocolate"
            value="Chocolate"
            v-model="cakeNames"
          />
          <span><i class="fas fa-check on"></i></span>
          <label for="chocolate"></label>
          
        </label>
      </div>

      <div class="cakeSelection">
        <img src="../assets/fresa.jpg" alt="" />
        <h3>Fresa</h3>
        <label class="mycheckbox">
          <input
            type="checkbox"
            id="fresa"
            value="Fresa"
            v-model="cakeNames"
          />
          <span><i class="fas fa-check on"></i></span>
          <label for="fresa"></label>
        </label>
      </div>

      <div class="cakeSelection">
        <img src="../assets/cajeta.jpg" alt="" />
        <h3>Cajeta</h3>
        <label class="mycheckbox">
          <input
            type="checkbox"
            id="cajeta"
            value="Cajeta"
            v-model="cakeNames"
          />
          <span><i class="fas fa-check on"></i></span>
          <label for="cajeta"></label>
        </label>
      </div>

      <br />
    </div>
    <div class="cakeContainer">
      <div class="cakeSelection">
        <img src="../assets/moras.jpg" alt="" />
        <h3>Moras</h3>
        <label class="mycheckbox">
          <input
            type="checkbox"
            id="moras"
            value="Moras"
            v-model="cakeNames"
          />
          <span><i class="fas fa-check on"></i></span>
          <label for="moras"></label>
        </label>
      </div>

      <div class="cakeSelection">
        <img src="../assets/oreo.jpg" alt="" />
        <h3>Oreo</h3>
        <label class="mycheckbox">
          <input
            type="checkbox"
            id="oreo"
            value="Oreo"
            v-model="cakeNames"
          />
          <span><i class="fas fa-check on"></i></span>
          <label for="oreo"></label>
        </label>
      </div>

      <div class="cakeSelection" id="container">
        <img src="../assets/red-velvet.jpg" alt="" />
        <h3>Red velvet</h3>
        <label class="mycheckbox">
          <input
            type="checkbox"
            id="red velvet"
            value="Red velvet"
            v-model="cakeNames"
          />
          <child :checkbox="cakeNames"></child>
          <span><i class="fas fa-check on"></i></span>
          <label for="red velvet"></label>
        </label>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data(){
    return {
      cakeNames: []
    }
  }
}
</script>

<style lang="scss">
.tituCake {
  color: #642a73;
  font-size: 30px;
  text-align: center;
  margin-bottom: 30px;
}

.combi {
  background: #fff;
  margin-top: 80px;
}
.listsCake {
  margin-left: 100px;
}

.cakeContainer {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
}

.cakeContainer h3{
    color: #642a73;
    font-size: 20px;
    text-align: center;
    margin-top: 5px;
    margin-bottom: 5px
}

.cakeSelection {
    text-align: center;
  width: 300px;
  height: 300px;
  margin-top: 50px;
  margin-bottom: 50px;
  overflow: unset;
  position: relative;
  box-shadow: 0 0 6px 0 rgba(0, 0, 0, 0.5);
}

.cakeSelection > img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.mycheckbox input:checked ~ span::after {
  background: rgba(9, 112, 9, 0.666);
  transform: scale(0.85) translate(35px);
}
.mycheckbox input:checked ~ span .on {
  transform: translate(30px);
  opacity: 1;
}

.mycheckbox input:checked ~ span .off {
  transform: translate(30px);
  opacity: 0;
}

.mycheckbox input {
  display: none;
}

.mycheckbox span {
  display: inline-block;
  width: 60px;
  height: 30px;
  border-radius: 30px;
  background: rgba(182, 26, 196, 0.254);
  cursor: pointer;
  box-shadow: inset 0px 0px 2px rgb(15, 15, 15);

  position: relative;
}

.mycheckbox span::after {
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

.mycheckbox i {
  position: absolute;
  left: 7px;
  top: 7px;
  z-index: 1;
  color: white;
  transition: 0.5s;
}

.mycheckbox .on {
  opacity: 0;
  left: 7px;
  top: 7px;
}

.mycheckbox .off {
  left: 9px;
  top: 7px;
}
</style>
