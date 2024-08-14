<template>
    <div>
      <h1 data-aos="fade-up">Hello, AOS!</h1>
      <p data-aos="fade-right">This is a paragraph with a right fade animation.</p>
    </div>
  </template>
  
  <script>
  export default {
    mounted() {
      // Refresh AOS after the component is mounted
      this.$nextTick(() => {
        AOS.refresh();
      });
    },
  };
  </script>
  
  <style scoped>
  /* Your component-specific styles here */
  </style>
  