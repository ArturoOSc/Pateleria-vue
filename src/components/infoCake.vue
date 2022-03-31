<template>
<h1 class="tituInfo">Realiza tu pedido</h1>
    <section class="form-register"> 
    <h4>Formulario de pedido</h4>
    <input class="controls" type="text" name="nombres" id="nombres" placeholder="Nombre(s)">
    <input class="controls" type="text" name="apellidos" id="apellidos" placeholder="Apellido(s)">
    <input class="controls" type="email" name="correo" id="correo" placeholder="Correo: micorreo@example.com">
    <input class="controls" type="telephone" name="telefono" id="telefono" placeholder="Teléfono">
    <p>Estoy de acuerdo con <a href="#">Terminos y Condiciones</a></p>
    <input class="botons" type="submit" value="Registrar">
    <span>Selecciono: {{checkbox}} </span>
    <p><a href="#">¿Ya tengo Cuenta?</a></p>
  </section>

</template>

<script>
import infoCake from "@/components/infoCake.vue"
export default {
    components:{
    infoCake
  },
  props: ['checkbox']
    
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.tituInfo {
  color: #642a73;
  font-size: 30px;
  text-align: center;
  margin-top: 40px;
  background: #728b8f56;
}

.form-register {
  width: 400px;
  background: #160b5ef8;
  padding: 30px;
  margin: auto;
  margin-top: 20px;
  border-radius: 4px;
  font-family: 'calibri';
  color: white;
  box-shadow: 7px 13px 37px rgba(184, 33, 214, 0.529);
}

.form-register h4 {
  font-size: 22px;
  margin-bottom: 20px;
}

.controls {
  width: 100%;
  background: #fff;
  padding: 10px;
  border-radius: 4px;
  margin-bottom: 16px;
  border: 1px solid #fff;
  font-family: 'calibri';
  font-size: 18px;
  color: white;
}

.controls #placeholder{
    color: #fff;
}


.form-register p {
  height: 40px;
  text-align: center;
  font-size: 18px;
  line-height: 40px;
}

.form-register a {
  color: white;
  text-decoration: none;
}

.form-register a:hover {
  color: white;
  text-decoration: underline;
}

.form-register .botons {
  width: 100%;
  background: #dc0ca1fd;
  border: none;
  padding: 12px;
  color: white;
  margin: 16px 0;
  cursor: pointer;
  font-size: 16px;
}
</style>