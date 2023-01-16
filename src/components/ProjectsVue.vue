


<template>

<div class="projects" >
        <div class="container" >
              <div class="card" style="width: 300px;height: 400px; margin: 10px;" v-for="item in projects">
                <div class="card-body">
                    <img :src="item.image"  class="card-img-top" alt="...">
                  <h5 class="card-title bold">{{ item.name }}</h5>     
                  <div class=" d-grid gap-2 col-6 mx-auto">
                  <a class="btn btn-dark" :href="item.netlify" target="_blank_">netlify</a>
                  <a  class="btn btn-dark" :href="item.github" target="_blank_">github</a>
                </div>
                  </div>
                </div>
             </div>
     </div>





</template>


<script>

export default {
data() {
   return {
   projects: [
  {
  title:'netflix',
  image:'https://i.postimg.cc/VkQMbcTw/netflix.jpg',
  description:"netflix clone",
  github:'https://github.com/siwere66087/netflix-clone.git',
  netlify:'https://genuine-granita-7ae8d1.netlify.app/'

  },
  {
  title:'calculator',
  image:'https://i.postimg.cc/jSJccHYP/IMG-20221019-WA0017.jpg',
  description:"web calculator ",
  github:'https://github.com/siwere66087/calculatorJs.git',
  netlify:'https://siwecalculator.netlify.app'

  },
  {
  title:'clothing store',
  image:'https://i.postimg.cc/Z5N6z1VS/fashion-5320934-1920.jpg',
  description:"",
  github:'https://github.com/siwere66087/clothingstore.git',
  netlify:''

  },
  {
  title:'ecommerce',
  image:'https://i.postimg.cc/L5bF8586/jacket-32714-1280.png',
  description:"jacket store",
  github:'https://github.com/siwere66087/ecommerse.git',
  netlify:'jacketzz.netlify.app'

  },
  {
  title:' js portfolio',
  image:'https://i.postimg.cc/jSJccHYP/IMG-20221019-WA0017.jpg',
  description:"portfolio",
  github:'https://github.com/siwere66087/submit-pos.git'


  },
  {
  title:'bs portfolio',
  image:'https://i.postimg.cc/jSJccHYP/IMG-20221019-WA0017.jpg',
  description:"personal bs portfolio",
  github:'https://github.com/siwere66087/bs-portfolio.git',
  netlify:''

  }
]

   }
},
}





</script>




<style>


.container{
    display: grid; 
    grid-template-columns: 1fr 1fr 1fr;
    align-items: center  !important;;
    
  }
.projects{
    padding-top: 125px;
   
    
 
}
 @media only screen and (max-width:970px) {
  .container{
    margin-top: 30px;
    display: grid; 
    grid-template-columns: 1fr 1fr;
    
  }
}
@media only screen and (max-width: 580px) {
  .container{
    display: grid; 
    grid-template-columns: 1fr;
    
  }
}
img{
  height: 12rem;
  object-fit: cover;
}
.btn::after {
  position: absolute;
  top: 25px;
  left: 0;
  content: "";
  width: 0%;
  height: 3px;
  background-color: rgba(255, 255, 255, 0.6);
  transition: all 0.5s;
}

.btn:hover::after {
  width: 100%;
}




/* RESPONSIVE */

@media (max-width: 1600px) {
  .card {
    justify-content: center;
  }
}

</style>

