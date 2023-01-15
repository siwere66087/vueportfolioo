


<template>
  

<!-- left content -->

   <div class="container"  v-for="item in personalDetails" :key="item">
    <img :src="item.image" class="img">
 <div class="card-body">
  <h1 id="title">{{ item.title }}</h1>
  <h1 id="titlle">{{ item.post }}</h1>
  <button type="button" class="button btn"><a href="#about" >about me</a></button>
 </div>


      </div>
<!-- right content -->
   <section id="home"  >

<div class="text-wrapper">
  <h2>I am a <span></span></h2>
 <a href="#">hire me</a>
 
 </div>
 
 <div id="social-icons">
  <li><a href="" id="icons"><i class="  fa-brands fa-facebook"></i> </a></li>
  <li><a href="" id="icons"><i class="fa-brands fa-twitter"></i> </a></li>
  <li><a href="" id="icons"><i class="fa-brands fa-linkedin"></i> </a></li>
  <li><a href="" id="icons"><i class="fa-brands fa-instagram"></i> </a></li>
 
 </div>
  </section>



</template>





<script>

export default {
 data() {
  return {
    // name:'card',
    personalDetails:[]
  }
 },
 mounted() {
  this.personalDetails = [{
  title:'siwe cele',
  post:'front-end-developer',
  image:'https://i.postimg.cc/jSJccHYP/IMG-20221019-WA0017.jpg'


  }]

 
 }
}
</script>



<style scoped>
button a{
  font-size: 19px;
  letter-spacing: 1px;
  transform: translateZ(-25px);
  transition: transform .25s;
  font-family:  sans-serif;
  
}
.titlle{
 color: #fff;
 font-size: 20px;
 text-transform: uppercase;
}
/* left content */
#title{
  color: white;
  font-size: 22px;
}
button{
  position: relative;
  display: inline-flex;
  width: 180px;
  height: 55px;
  margin: 0 15px;
  perspective: 1000px;
 }
 button a{
  font-size: 19px;
  letter-spacing: 1px;
  transform-style: preserve-3d;
  transform: translateZ(-25px);
  transition: transform .25s;
  font-family: 'Montserrat', sans-serif;
  
 }
 button  a:before,
 button a:after{
  position: absolute;
  content: "about me";
  height: 55px;
  width: 180px;
  display: flex;
  align-items: center;
  justify-content: center;
  border: 5px solid black;
  box-sizing: border-box;
  border-radius: 5px;
}
button a:before{
  color: #fff;
  background: rgb(86, 11, 11);
  transform: rotateY(0deg) translateZ(25px);
}
button  a:after{
  color: rgb(255, 255, 255);
  transform: rotateX(90deg) translateZ(25px);
}
button  a:hover{
  transform: translateZ(-25px) rotateX(-90deg);
}

img {
  width: 30%;
  height: 100%;
  object-fit:cover;
  
  -webkit-box-reflect:below 2px linear-gradient(transparent, transparent, #0004);
  
  transform-origin:center;
  transform:perspective(800px) rotateY(25deg);
  transition:0.5s;
}
.container {
width: 50%;;
 height: 60vh;
display: block;
margin-right: 90rem;
border:2px solid red;

  
}
.container:hover img {
  opacity:0.9;
}
.container img:hover {
  transform:perspective(800px)  rotateY(0deg);
  opacity:1;
}


/* right content */

#home{

width: 40rem;
border: 3px solid grey;
height: 34rem;
margin-left: 45rem;
position: relative;
}
.text-wrapper{ 
position: relative;
top: 30px;


}

.text-wrapper h2{
padding: 0;
margin: 0;
color: rgb(240, 87, 87);
text-shadow: 0 2px 0 rgba(0, 0, 0, 0.5);
font-size: 50px;

}

.text-wrapper a{
color: white;
text-decoration: none;
padding: 10px 25px;
display: inline-block;
border-radius: 5px;
margin-top: 30px;
box-shadow: firebrick;
border: 2px solid red;
}

span::before{
content: "";
animation: animate 6s infinite;

}
@keyframes animate {

0%{
    content: 'web developer';
}
20%{
    content: 'graphic designer';
}
40%{
    content: 'freelancer';
}
60%{
    content: 'web developer';
}
80%{
    content: 'fullstack ';
}
100%{
    content: 'web designer';
}
}

#social-icons{
width: 550pxx;
height: 10vh;
margin-top: 320px;
margin-left: 40px;
display: inline-flex;
border: 2px solid rgb(225, 111, 111);
}
#social-icons li{
    list-style: none;
}
#social-icons li a{
color: white;
font-size: 30px;
padding: 15px;
margin-left: 60px;
margin-top: 30px;
}

#icons{
border-radius: 50px;
}




</style>
