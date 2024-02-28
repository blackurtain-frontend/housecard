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
  
  <style>
.card {
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  border: 3px black solid;
  border-radius: 15px;
  background-color: brown;
  text-align: center;
  display: inline-block;
  margin: 10px;
  height: 300px; 
  width: 80%;
  }
  .photo{
    clip: auto;
    height: 50%;
    width: 100%;
    margin-bottom: 20px;
    border-radius: 15px;
  }
  .photo img {
    width: 100%;
    size: 30px;
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
  