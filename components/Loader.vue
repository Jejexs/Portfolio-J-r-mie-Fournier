<template>
 
    <div v-if="isLoading" class="loader">
      <img src="../assets/img/time.png" alt="">

      <div class="loader-spinner absolute">
        <img src="../assets/img/developpeur.png" alt="">
      </div>
      
    </div>
  </template>
  
  <script>
export default {
  data() {
    return {
      isLoading: true,
    }
  },
  mounted() {
    setTimeout(() => {
      this.isLoading = false
      this.$router.push('/')
    }, 2000)

    window.addEventListener('load', () => {
      this.isLoading = false
    })
  },
}
</script>
  
  <style>
  .loader {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 9999;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #b7b7b7;
  }
  
  .loading .loader {
    opacity: 0;
    visibility: hidden;
  }
  
  .loader-spinner {
    display: block;
    width: 150px;
    height: 150px;
    border-radius: 50%;
    border: 4px solid #ffffff;
    border-top-color: #00b7ff;
    animation: spin 1s ease-in-out infinite;
  }
  
  @keyframes spin {
    0% {
      transform: rotate(0);
    }
    100% {
      transform: rotate(360deg);
    }
  }
  </style>
  