


<template>

<section class="project" id="project" >

<!-- item.heading -->
<div class="heading">
    <span>projects</span>
   
</div>

<div class="box-container" v-for="item in projects"  :key="item">

    <div class="box" data-aos="fade-up" data-aos-delay="150" >
      <img :src="item.image" class="img">
            
        </div>
        <div class="content">
            <h3>{{item.title}}</h3>
            <p>{{item.description}}</p>
            <div class="iconCont">
            <a href="item.github">github <i class="fas fa-angle-right"> </i></a>
            <a href="item.netlify">netlify <i class="fas fa-angle-right"></i></a>
          </div>
          </div>
    </div>
    </section>
  
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
  github:'',
  netlify:''

  },
  {
  title:'netflix',
  image:'https://i.postimg.cc/jSJccHYP/IMG-20221019-WA0017.jpg',
  description:"netflix clone",
  github:'',
  netlify:''

  },
  {
  title:'netflix',
  image:'https://i.postimg.cc/jSJccHYP/IMG-20221019-WA0017.jpg',
  description:"netflix clone",
  github:'',
  netlify:''

  },
  {
  title:'netflix',
  image:'https://i.postimg.cc/jSJccHYP/IMG-20221019-WA0017.jpg',
  description:"netflix clone",
  github:'',
  netlify:''

  },
  {
  title:'netflix',
  image:'https://i.postimg.cc/jSJccHYP/IMG-20221019-WA0017.jpg',
  description:"netflix clone",
  github:'',
  netlify:''

  }

]

   }
},
}





</script>




<style>



.project .box-container {
 
 display: grid;
grid-template-columns: repeat(3,1fr);
 /* -ms-grid-columns: (minmax(27rem, 1fr))[auto-fit]; */
 grid-template-columns: repeat(auto-fit, minmax(3, 1fr));
 gap: 1.5rem;
}

.project .box-container .box {
 border-radius: 1rem;
 overflow: hidden;
 background: #222;
}

.project .box-container .box:hover img {
 -webkit-transform: scale(1.1);
         transform: scale(1.1);
}

.project.box-container .box .image {
 height: 20rem;
 overflow: hidden;
 width: 100%;
}

.project .box-container .box .image img {
 height: 100%;
 width: 100%;
 object-fit: cover;
}

.project .box-container .box .content {
 padding: 2rem;
 text-align: center;
}

.project .box-container .box .content h3 {
 font-size: 2rem;
 color: #fff;
}

.project .box-container .box .content p {
 padding: 1rem 0;
 font-size: 1.4rem;
 color: #aaa;
 line-height: 2;
}

.project .box-container .box .content a {
 font-size: 1.7rem;
 color: #29d9d5;
}

.project .box-container .box .content a:hover i {
 padding-left: 1rem;
}

.project .box-container .box .content a i {
 padding-right: .5rem;
}

.btn{
   display: inline-block;
   margin-top: 1rem;
   background-color: rgb(160, 60, 118);
   cursor: pointer;
   color:white;
   border: #29d9d5 3px solid;
   font-size: 1.8rem;
   padding:1rem 3rem;
}

.btn:hover{
   background-color: black;
}

#project-btn{
   display: none;
   font-size: 2.5rem;
   color:black;
   cursor: pointer;
}




/* media queries  */

@media (max-width:991px){

html{
   font-size: 55%;
}

}

@media (max-width:768px){

  #project{
   display: inline-block;
   transition: .2s linear;
}

#project.fa-times{
   transform: rotate(180deg);
}


}

@media (max-width:450px){

html{
   font-size: 50%;
}

img{
   height: 3rem;
}

 h3{
   font-size: 3rem;
}

}
</style>

