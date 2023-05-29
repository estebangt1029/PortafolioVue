<script>
import Modal from '@/components/Modal.vue';
  export default {
    components: {
    Modal
  },
  data() {
    return {
      showModal: false,
      modalTitle: 'Título del modal',
      modalMessage: 'Contenido del modal',
      repo:'repositorio'
    };
  },
    props: {
      image: {
        type: String,
        required: true
      },
      title: {
        type: String,
        required: true
      },
      description: {
        type: String,
        required: true
      },
      repo: {
        type: String,
        required: true
      }
    }
  }
</script>
<template>
    <div class="projects">
        <img :src="image" alt="">
        <!-- <h2>{{ title }}</h2>
        <p>{{ description }}</p> -->
        <div>
          <svg @click="showModal = true" xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="darkgray" class="bi bi-info-circle-fill" viewBox="0 0 16 16">
            <path d="M8 16A8 8 0 1 0 8 0a8 8 0 0 0 0 16zm.93-9.412-1 4.705c-.07.34.029.533.304.533.194 0 .487-.07.686-.246l-.088.416c-.287.346-.92.598-1.465.598-.703 0-1.002-.422-.808-1.319l.738-3.468c.064-.293.006-.399-.287-.47l-.451-.081.082-.381 2.29-.287zM8 5.5a1 1 0 1 1 0-2 1 1 0 0 1 0 2z"/>
          </svg>
          <Modal :title="title" :message="description" :repositorio="repo" :show-modal="showModal" @close="showModal = false" />
        </div>
    </div>
</template>
<style scoped>
    .projects{
        width: 100%;
        text-align: center;
        position: relative;
    }
    img{
      width: 90%;
      box-shadow: 0 0 10PX 5px rgba(255, 255, 255, 0.534);
    }
    .bi{
      position: absolute;
      bottom: 10px;
      right: 6%;
      cursor: pointer;
    }
</style>