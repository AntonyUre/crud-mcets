<template>
  <div class="home">
    <div class="wrapper">
    <header>
      <nav>
        <a href="https://antonyur.com/" target="_blank">
          <img src="@/assets/img/Logo-mcets.svg" alt="">
        </a>
        <div>
          <button id="crear" class="btn open-modal" @click="open">Agregar Usuario</button>
        </div>
      </nav>
    </header>

    <div class="list-container">
      <div class="text-container">
        <h2>Lista de usuarios</h2>
        <p><span>0 </span>Usuarios </p>
      </div>

      <div class="list-items">
        <div class="user">
          <p>Antony Ureta Acuña</p>
          <p>24 años</p>
          <p>75552715</p>
          <p>Perú</p>
          <div class="icons">
            <i class="far fa-edit"></i>
            <i class="far fa-trash-alt"></i>
          </div>
        </div>
      </div>
    </div>
  </div>
  <ModalCreate v-if='open_modal'/>
  </div>
</template>

<script>
// @ is an alias to /src
import ModalCreate from '@/components/ModalCreate.vue';

export default {
  name: 'Home',
  components: {
    ModalCreate,
  },
  data() {
    return {
    open_modal: false,
    };
  },
  methods: {
    open(){
      this.open_modal=true;
    }
  },
};
</script>
<style lang="scss">

</style>
