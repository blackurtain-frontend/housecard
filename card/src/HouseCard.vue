<template>
    <div class="card">
      <div class="photo">
        <img src="istock.jpeg" alt="House Photo" />
      </div>
      <div class="details">
        <h2>{{ house.name }}</h2>
        <p><strong>Location:</strong> {{ house.location }}</p>
        <p><strong>Type:</strong> {{ house.type }}</p>
        <p><strong>Price:</strong> {{ house.price }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'HouseCard',
    props: {
      house: {
        type: Object,
        required: true
      }
    }
  }
  </script>
  
  <style scoped>
.card {
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  border: 3px black solid;
  border-radius: 15px;
  background-color: brown;
  text-align: center;
  }
  
  .photo img {
    max-width: 50%;
    height: auto;
  }
  
  .details {
    flex: 2;
    padding: 0 20px;
  }
  
  h2 {
    margin-top: 0;
  }
  
  p {
    margin: 5px 0;
  }
  </style>
  