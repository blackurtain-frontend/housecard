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
        name: 'Beautiful Villa',
        location: 'City, Country',
        type: 'Villa',
        price: '$500,000'
      }
    };
  }
};
</script>
