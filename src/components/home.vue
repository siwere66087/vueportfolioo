


<template>
  

<div class="wrapper" style="background-color: black;">
    <div class="profile" v-for="item in personalDetails" :key="item">
        <div class="overlay">
            <div class="about d-flex flex-column">
                <h2>{{item.title}}</h2> 
                <span>{{ item.post }}</span>
            </div>
            
            <ul class="social-icons">
                <li><i class=" fab  fa-brands fa-facebook " ></i></li>
                <li><i class=" fab  fa-brands fa-twitter" ></i></li>
                <li><i class=" fab  fa-brands fa-github" ></i></li>
                <li><i class=" fab  fa-brands fa-linkedin" ></i></li>
            </ul>

           <a href="#about" class="button" >About me</a>
        </div>
    </div>
</div>


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
.wrapper{
display: flex;
justify-content: center;
align-items: center;
height: 100vh;
width: 100vw;
background:#000;
position: fixed;
}
.profile{
   position: relative;
   width: 350px;
   height: 400px;
   background:url("https://i.postimg.cc/jSJccHYP/IMG-20221019-WA0017.jpg");
   background-size: cover;
   cursor: pointer;
   border: 10px;
   border-top-right-radius: 35px !important;
   border-radius: 6px
   }
   .overlay{
      width: 100%;
      height: 100%;
      background:rgba(0,0,0,0.8);
      border-radius: 12px;
      cursor: pointer;
      opacity: 0;
      transition: all 1s;
      border-top-right-radius: 35px !important;
      border-radius: 6px
      }
      .profile:hover .overlay{
         opacity: 1
         }
         .social-icons{
            display: flex;
            list-style: none;
            bottom: 10px;
            position: absolute;
            text-align: center;
            justify-content: center;
            left: 22px
            }
            .social-icons li{
               width: 25px;
               height: 25px;
               border: 1px solid #eee;
               padding: 20px;
               margin-right: 10px;
               display: flex;
               justify-content: center;
               align-items: center;
               color: #fff;
               border-radius: 5px;
               transition: all 1s
               }
               .social-icons li:hover{
                  background:#fff;
                  color: #000
                  }
                  .overlay .about{
                     position: relative;
                     justify-content: center;
                     align-items: center;
                     display: flex;
                     top:40%;
                     color: #fff;
                     flex: column
                     }


.button {
display: inline-block;

font-size: 16px;
cursor: pointer;
text-align: center;
text-decoration: none;
margin-top: 12rem;
outline: none;
color: white;
background-color: rgb(58, 57, 57);
border: none;
border-radius: 15px;

}
.button:hover {background-color: rgb(226, 66, 8)}
.button:active {
background-color: rgb(134, 226, 20);
transform: translateY(4px);
}


</style>
