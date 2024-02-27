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
    border: 1px solid #ccc;
    border-radius: 5px;
    display: inline-block;
    width:fit-content; 
    box-shadow:20px;
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
  