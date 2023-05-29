<template>
    <div class="modal" v-if="showModal">
      <div class="modal-content">
        <h2>{{ title }}</h2>
        <p>{{ message }}</p>
        <a href="{{ repositorio }}">Repositorio</a>
        <a href="">Web</a>
        <button @click="closeModal">Cerrar</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      title: String,
      message: String,
      repositorio: String,
      showModal: Boolean
    },
    methods: {
      closeModal() {
        this.$emit('close');
      }
    }
  };
  </script>
  
  <style scoped>
  .modal {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5);
    display: flex;
    align-items: center;
    justify-content: center;
    z-index: 10;
  }
  
  .modal-content {
    background-color: darkgray;
    padding: 2rem;
    border-radius: 8px;
    width: 50%;
    min-height: 50%;
    display: grid;
    place-items: center;
  }
  @media only screen and (max-width: 768px) {
.modal-content {
    width: 100%;
    min-height: 100%;
  }
}
  
  a{
    text-decoration: none;
    color: blueviolet;
  }
  button {
    margin-top: 1rem;
    cursor: pointer;
    background-color: black;
    color: white;
    border: none;
    padding: 10px 20px;
    border-radius: 12px;
  }
  </style>
  