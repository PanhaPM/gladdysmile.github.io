<script setup>
import { ref, computed, nextTick } from 'vue';

const showMenu = ref(false);
const text1 = ref("On 18. 07. 2024-is the date I was created this website by myself,");
const text2 = ref("It's the second website I was created before since I was study Information Technology.");
const text3 = ref(""); // Initially empty
const name = ref("Testing Website");

const toggleMenu = () => {
    showMenu.value = !showMenu.value;


    if (showMenu.value) {
        text1.value = "";
        text2.value = "";
        name.value = "";
        setTimeout(() => {
            text3.value = "Soun Panha";
        }, 1000); // Delay of 1 second
    } else {
        text1.value = "On 18. 07. 2024-is the date I was created this website by myself,";
        text2.value = "It's the second website I was created before since I was study Information Technology.";
        name.value = "Testing Website";
        text3.value = "";
    }
};

const overlayStyle = computed(() => ({
    background: showMenu.value ? 'rgba(0, 0, 0, 0.740)' : 'rgba(0, 0, 0, 0.5)',
}));
</script>

<template>
    <div>
        <div class="hero-section">
            <img src="/src/assets/img/about 7.jpg" alt="Background Image" class="background-image">
            <div class="overlay" :style="overlayStyle">
                <h1></h1>
                <transition name="fade" @before-enter="beforeEnter" @enter="enter" @leave="leave">
                    <span v-if="!showMenu">{{ name }}</span>
                </transition>
                <transition name="fade" @before-enter="beforeEnter" @enter="enter" @leave="leave">
                    <p v-if="!showMenu" class="text1">{{ text1 }}</p>
                </transition>
                <transition name="fade" @before-enter="beforeEnter" @enter="enter" @leave="leave">
                    <p v-if="!showMenu" class="text2">{{ text2 }}</p>
                </transition>
                <transition name="fade-delayed">
                    <p v-if="showMenu" class="text3">{{ text3 }}</p>
                </transition>
                <transition>
                    <i v-if="!showMenu" class="fa-solid fa-ellipsis menu" @click="toggleMenu"></i>
                </transition>
                <transition>
                    <i v-if="showMenu" class="fa-solid fa-xmark close" @click="toggleMenu"></i>
                </transition>
                
            </div>
        </div>
    </div>
</template>

<style scoped>
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
.hero-section {
    position: relative;
    width: 100%;
    height: 100%; /* Adjust the height as needed */
    outline: none;
    overflow: hidden;
}

.background-image {
    width: 100%;
    height: 911px;
    object-fit: cover;
}

.overlay {
    position: absolute;
    width: 100%;
    height: 911px;
    top: 0;
    overflow: hidden;
    color: white;
    z-index: 33;
    transition: background 1s ease; /* Smooth transition */
}

h1 {
    font-size: 2.5em;
    margin-bottom: 10px;
}

p, span {
    font-size: 1.2em;
}

span {
    position: absolute;
    font-size: 70px;
    font-weight: bold;
    color: white;
    z-index: 50;
    margin-top: 380px;
    margin-left: 710px;
    width: 100%;
}

.text1, .text2 {
    font-family: "Caveat", cursive;
    font-optical-sizing: auto;
    font-weight: 500;
    font-style: normal;
    position: absolute;
    font-size: 19px;
    color: white;
}

.text1 {
    margin-left: 680px;
    margin-top: 490px;
}

.text2 {
    margin-left: 550px;
    margin-top: 530px;
}

.text3 {
    font-family: "Caveat", cursive;
    font-optical-sizing: auto;
    font-weight: 500;
    font-style: normal;
    position: absolute;
    font-size: 30px;
    color: white;
    font-weight: bold;
    margin-left: 880px;
    margin-top: 430px;
}

i {
    position: absolute;
    right: 80px;
    bottom: 40px;
    cursor: pointer;
}

.menu {
    font-size: 30px;
}

.close {
    font-size: 30px;
}

/* Transition effects */
.fade-enter-active, .fade-leave-active {
    transition: opacity 0.6s ease, transform 0.6s ease;
}

.fade-enter, .fade-leave-to {
    opacity: 0;
    transform: translateY(100px); /* Adjust as needed */
}

.fade-delayed-enter-active {
    transition: opacity 0.6s ease 1s, transform 0.6s ease 1s; /* 1 second delay */
}

.fade-delayed-enter, .fade-delayed-leave-to {
    opacity: 0;
    transform: translateY(100px); /* Adjust as needed */
}
</style>
