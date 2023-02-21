<template>
    <div>
      <button v-if="checkInDate !== today" @click="checkIn">Check In Today</button>
    </div>
  </template>
  
  <style>
  button {
    background-color: blue;
    color: white;
    padding: 10px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  </style>
<script>
export default {
    data() {
  return {
    checkInDate: null
  };
},

mounted() {
  const today = new Date().toLocaleDateString()
  if (this.checkInDate !== today) {
    // User has not checked in today
    // Display check-in button
  }
},
methods: {
  checkIn() {
    // Update check-in date to today
    this.checkInDate = new Date().toLocaleDateString()
    // Perform any other check-in related tasks
  }
}

  };


</script>

    