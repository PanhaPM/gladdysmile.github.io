<template>
    <div id="app">
      <button @click="toggleSidebar" class="openbtn">
        <a>Categories</a>
      </button>
      <div class="sidebar" :class="{ open: isSidebarOpen }">
        <button @click="toggleSidebar" class="closebtn">
          <i class="fa-solid fa-xmark"></i>
        </button>
        <RouterLink to="/ingredient"><a>Home</a></RouterLink>
        <RouterLink to="/ingredient"><a>Home</a></RouterLink>
        <RouterLink to="/ingredient"><a>Home</a></RouterLink>
        <RouterLink to="/ingredient"><a>Home</a></RouterLink>
        <RouterLink to="/ingredient"><a>Home</a></RouterLink>
        <RouterLink to="/ingredient"><a>Home</a></RouterLink>
        <RouterLink to="/ingredient"><a>Home</a></RouterLink>
        <RouterLink to="/ingredient"><a>Home</a></RouterLink>
        <RouterLink to="/ingredient"><a>Home</a></RouterLink>
        <RouterLink to="/ingredient"><a>Home</a></RouterLink>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        isSidebarOpen: false,
      };
    },
    methods: {
      toggleSidebar() {
        this.isSidebarOpen = !this.isSidebarOpen;
      },
    },
  };
  </script>
  
  <style>
  body {
    font-family: "Lato", sans-serif;
    text-decoration: none;
    margin: 0;
  }
  
  .openbtn {
    background: none;
    border: none;
    padding: 10px 20px;
    position: absolute;
    top: 20px;
    left: 20px;
  }
  
  .openbtn a {
    position: absolute;
    margin: 0;
    font-size: 18px;
    font-weight: 500;
    color: black;
    margin-top: -39px;
    margin-left: -110px;
  }
  
  .sidebar {
    position: absolute;
    height: 100%;
    width: 0;
    position: fixed;
    cursor: auto;
    z-index: 1;
    top: 0;
    left: 0;
    background-color: whitesmoke;
    overflow-x: hidden;
    transition: 0.3s;
    margin-top: 40px;
    padding-top: 60px;
    z-index: 9999;
  }
  .sidebar i{
    color: black;
    font-size: 25px;
    font-weight: bold;
    margin-top: 30px;
    padding-right: 10px;
  }
  
  .sidebar.open {
    width: 350px;
    cursor: auto;
  }
  
  .sidebar a {
    text-decoration: none;
    font-size: 18px;
    display: block;
    color: black;
    transition: 0.3s;
    padding-top: 15px;
    padding-left: 70px;
    font-weight: bold;
    cursor: auto;
  }

  .sidebar a:hover{
    cursor: pointer;
  }
  
  
  .sidebar .closebtn {
    position: absolute;
    top: 0;
    right: 25px;
    font-size: 36px;
    background: none;
    border: none;
  }
  
  .content {
    transition: margin-left 0.5s;
    padding: 16px;
  }
  
  .shift-right {
    margin-left: 250px;
  }
  </style>
  