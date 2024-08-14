<template>
    <body>
    <div class="logo-container">
        <img src="/src/assets/img/Logo no background.png" alt="Logo" class="logo">
    </div>
</body>
</template>

<style scoped>
 /* styles.css */
body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #fff;
    margin: 0;
}

.logo-container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: auto; /* Adjust the height as needed */
    width: 250px; /* Adjust the width as needed */
    object-fit: cover;
}

.logo {
    width: 100%;
    height: 100%;
    animation: fadeInOut 4s infinite;
}

@keyframes fadeInOut {
    0%, 100% {
        opacity: 0;
    }
    50% {
        opacity: 1;
    }
}


</style>

<script setup>
    // script.js
document.addEventListener('DOMContentLoaded', () => {
    const logo = document.querySelector('.logo');
    
    // Example: Stop animation after 5 seconds
    setTimeout(() => {
        logo.style.animation = 'none';
    }, 5000);
});

</script>