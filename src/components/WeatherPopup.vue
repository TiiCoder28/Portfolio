<script>
export default {
  data() {
    return {
      isVisible: true, 
    };
  },
  methods: {
    redirectToWeatherApp() {
    
      window.location.href = "https://tiicoder28.github.io/weatherApp/";
    },
    closePopup() {
      
      this.isVisible = false;
    },
  },
};
</script>


<template>
    <div id="weather-popup" class="popup" v-if="isVisible">
      <div class="popup-content">
        <h3 class="heading vt323-regular">Welcome!</h3>
        <p class="vt323-regular">Would you like to know where you are and check the current weather?</p>
        <div class="popup-buttons">
          <button @click="redirectToWeatherApp" class="btn">Yes</button>
          <button @click="closePopup" class="btn">No</button>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  .popup {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.7);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 1000;
  }
  
.popup-content p{
    color: var(--main-color);
    font-size: 5rem;
}

  .popup-content {
    background: var(--secondary-color);
    padding: 2rem;
    border-radius: 10px;
    text-align: center;
    width: 90%;
    max-width: 400px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
  }
  
  .popup-buttons .btn {
    margin: 0.5rem;
    padding: 0.5rem 1.5rem;
    border: none;
    background: var(--main-color);
    color: white;
    border-radius: 5px;
    cursor: pointer;
    font-size: 3rem;
    border: 2px solid var(--main-color);
    box-shadow: 0 0 25px var(--main-color);
  }
  
  .popup-buttons .btn:hover {
    background: var(--secondary-color);
    transform: scale(1.03);
    transition: 0.3s ease-in-out;
  }
  </style>
  