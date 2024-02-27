<template>
    <div class="card">
      <div class="photo">
        <img src="card/public/istock.jpeg" alt="House Photo" />
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
    display: flex;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px;
    padding: 10px;
  }
  
  .photo {
    flex: 1;
  }
  
  .photo img {
    max-width: 100%;
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
  