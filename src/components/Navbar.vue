<template>

   <header class="header">
        
        <a href="#" class="logo">sm</a>

       
        <input class="side-menu" type="checkbox" id="side-menu"/>
        <label class="hamb" for="side-menu"><span class="hamb-line"></span></label>

        <!-- Menu -->
        <nav class="nav">
            <ul class="menu">
              <li><a class="nav-link scrollto active" href="#hero">
            <router-link to="/">Home</router-link>
          </a></li>
          <li><a class="nav-link scrollto" href="#about">
            <router-link to="/about">About</router-link>| |
          </a></li>
            <li><a class="nav-link scrollto" href="#resume">
            <router-link to="/resume">resume</router-link>| |
          </a></li>
            <li><a class="nav-link scrollto" href="#projects">
            <router-link to="/projects">projects</router-link>| |
          </a></li>
            <li><a class="nav-link scrollto " href="#testamonials">
            <router-link to="/testamonials">testamonials</router-link>| |
          </a></li>
          <li><a class="nav-link scrollto" href="#contact">
            <router-link to="/contact">contact</router-link>
          </a></li>

            </ul>
        </nav>
    </header>

    
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
  
a{
    text-decoration: none;
}

ul{
    list-style: none;
}

/* Header */
.header{
    background-color: black;
    box-shadow: 1px 1px 5px 0px gray;
    position: sticky;
    top: 0;
    width: 100%;
}

/* Logo */
.logo{
    display: inline-block;
    color: white;
    font-size: 60px;
    margin-left: 10px;

}

/* Nav menu */
.nav{
    width: 100%;
    height: 100%;
    position: fixed;
    background-color: black;
    overflow: hidden;
    
}

.menu a{
    display: block;
    font-size: 16px;
    color: white;
    text-transform: capitalize;

}

.menu a:hover{
    background-color: rgb(158, 51, 51);
}

.nav{
    max-height: 0;
    transition: max-height .5s ease-out;
}



.hamb{
    cursor: pointer;
    float: right;
    padding: 40px 20px;
}


.hamb-line {
    background: white;
    display: block;
    height: 2px;
    position: relative;
    width: 24px;
    
}

.hamb-line::before,
.hamb-line::after{
    background: white;
    content: '';
    display: block;
    height: 100%;
    position: absolute;
    transition: all .2s ease-out;
    width: 100%;
}

.hamb-line::before{
    top: 5px;
}

.hamb-line::after{
    top: -5px;
}


.side-menu {
    display: none;
}

/* Toggle menu icon */

.side-menu:checked  nav{
    max-height: 100%;
}

.side-menu:checked .hamb .hamb-line {
    background: transparent;
}

.side-menu:checked  .hamb .hamb-line::before {
    transform: rotate(-45deg);
    top:0;

}

.side-menu:checked  .hamb .hamb-line::after {
    transform: rotate(45deg);
    top:0;
}


/* Responsiveness */

@media (min-width: 768px) {
    .nav{
        max-height: none;
        top: 0;
        position: relative;
        float: right;
        width: fit-content;
        background-color: transparent;

    }

    .menu li{
        float: left;
    }

    .menu a:hover{
        background-color: transparent;
        color: gray;
        
    }
    
    .hamb{
        display: none;
    }

}


  </style>
  
