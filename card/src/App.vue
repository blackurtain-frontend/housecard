<template>
  <div>
    <house-card :house="houseData" />
  </div>
</template>

<script>
import HouseCard from './HouseCard.vue';

export default {
  name: 'App',
  components: {
    HouseCard
  },
  data() {
    return {
      houseData: {
        name: 'Cosy Bungalow',
        location: 'Nairobi',
        type: 'Bungalow',
        price: '500,000ksh'
      }
    };
  }
};
</script>
