<template>
  <div class="windows-modal">
    <div class="modal-container close">
      <p>
        Añadir Usuario
        <button class="close-modal">X</button>
      </p>
      <form action="" class="inputs">
        <div>
          <input class="medio" type="text" placeholder="Nombre" required/>
          <input class="medio" type="text" placeholder="Apellido"/>
        </div>
        <div>
          <input type="text" placeholder="Edad" />
          <input type="number" placeholder="Dni" />
          <select name="country">
            <option value=" ">País</option>
            <option>Perú</option>
            <option>Argentina</option>
            <option>México</option>
            <option>Usa</option>
          </select>
        </div>
        <div class="send">
          <button type="button" class="btn">Aceptar</button>
          <button type="button" class="btn">Cancelar</button>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ModalCreate',
};
</script>

<style>

</style>
