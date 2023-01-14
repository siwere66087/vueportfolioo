


<template>

 <div class="main-container" v-for="item in projects"  :key="item">
  <div class="heading">
   
    <h2 class="title">projects</h2>
  </div>
  <img :src="item.image" class="img">
  <div class="cards">
    <div class="card card-1">
     
     <h2 class="">{{item.title}}</h2>
      <h2 class="card__title">{{item.description}}</h2>
      <p class="card__apply">
        <a class="btn" href="item.github">github <i class="fas fa-arrow-right"></i></a>
        <a class="btn" href="item.netlify">netlify <i class="fas fa-arrow-right"></i></a>
      </p>
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
  description:portfolio",
  github:'https://github.com/siwere66087/submit-pos.git',
  netlifyhttps://curious-creponne-176988.netlify.app

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



.main-container {
  padding: 30px;
}

.heading {
  text-align: center;
}

.heading__title {
  font-weight: 600;
}

.heading__link {
  text-decoration: none;
}

.cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

.card {
  margin: 20px;
  padding: 20px;
  width: 500px;
  min-height: 200px;
  display: grid;
  grid-template-rows: 20px 50px 1fr 50px;
  border-radius: 10px;
  box-shadow: 0px 6px 10px rgba(0, 0, 0, 0.25);
  transition: all 0.2s;
}

.card:hover {
  box-shadow: 0px 6px 10px rgba(0, 0, 0, 0.4);
  transform: scale(1.01);
}




.card__exit {
  grid-row: 1/2;
  justify-self: end;
}

.card__icon {
  grid-row: 2/3;
  font-size: 30px;
}

.card__title {
  grid-row: 3/4;
  font-weight: 400;
  color: #ffffff;
}

.card__apply {
  grid-row: 4/5;
  align-self: center;
}

.card-1 {
  background: radial-gradient(#1fe4f5, #3fbafe);
}



/* RESPONSIVE */

@media (max-width: 1600px) {
  .cards {
    justify-content: center;
  }
}

.btn .card__exit,
.card__icon{
   display: inline-block;
   margin-top: 1rem;
   background-color: rgb(160, 60, 118);
   cursor: pointer;
   border: #29d9d5 3px solid;
   font-size: 1.8rem;
   padding:1rem 3rem;
     position: relative;
  text-decoration: none;
  color: rgba(255, 255, 255, 0.9);
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


</style>

