<template>

    <nav>
      <router-link to="/">Home</router-link> | |
      <router-link to="/about">About</router-link>| |
      <router-link to="/resume">resume</router-link>| |
      <router-link to="/projects">projects</router-link>| |
      <router-link to="/testamonials">testamonials</router-link>| |
      <router-link to="/contact">contact</router-link>
    </nav>
    <router-view/>
    <footer></footer>
  </template>
  
  <script>


  
  
  </script>
  
  
  
  
  <style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
  
  nav {
    padding: 30px;
    background-color: rgb(15, 13, 13);
    display: block;
    flex-direction: column;
  }
  
  nav a {
    font-weight: bold;
    color: #fbfbfc;
    text-decoration: none;
    text-transform: uppercase;
  }
  nav a:hover{
  color: red;
  
  }
  nav a.router-link-exact-active {
    color: #279dba;
  }
  </style>
  