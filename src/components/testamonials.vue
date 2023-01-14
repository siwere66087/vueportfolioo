<template>
  <section id="Projects" style="background-color: white;">
    <div class="position-relative d-flex align-items-center justify-content-center">
          <h2 class="display-2 text-uppercase text-black">Testamonials</h2>
        </div>
    <div class="container-fluid" id="carousel">
      <div id="carouselExampleDark" class="carousel carousel-dark slide" data-bs-ride="carousel">
        <div class="carousel-inner">
          <div class="carousel-item active" data-bs-interval="10000" v-for="item3 in project1"
            :key="item3">
            <img :src="item3.image" alt="ProjectPic" class="img-fluid w-25 m-auto" loading="lazy">
            <h3 class="mt-3 text-black"> {{ item3.projectName }}</h3>
            <p class="text-black">{{ item3.description }}</p>
            <form :action="item3.gitHub" method="get" target="_blank"><button class="project-btn">GitHub</button></form><br>
              <a :href="item3.netlify"><button>Netlify</button></a>
          </div>
          <div class="carousel-item" data-bs-interval="10000" v-for="item3 in project" :key="item3">
            <img :src="item3.image" alt="projectPic" class="img-fluid w-25 m-auto" loading="lazy">
            <h3 class="mt-3 text-black">{{ item3.projectName }}</h3>
            <p class="text-black">{{ item3.description }}</p>
            <form :action="item3.facebook" method="get" target="_blank"><button class="project-btn">GitHub</button></form><br>
              <a :href="item3.instagram"><button>Netlify</button></a>
          </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'ProjectComponent',
  data () {
    return {
      project1: [{
        image: 'https://i.postimg.cc/G272k9P4/C11-Nontobeko-Mhlongo-1.jpg',
        projectName: 'Nontobeko Mhlongo',
        description: ' siwe is great person with great personality. she is easy to talk too and rely on.',
        gitHub: 'https://github.com/Ntobe99/Nonto-vue-portfolio',
      
        
      }],
      project: [{
        image: 'https://i.postimg.cc/HkyBRyVC/Gift-Mahlangu.jpg',
        projectName: 'Gift Mahlangu',
        description: '',
      
      },
      {
        image: 'https://ca.slack-edge.com/T02LW4RMXJQ-U0444AHR59B-a9d9ad76f500-512',
        projectName: 'Sibabalwe',
        description: 'Some people are naturally outgoing, conversational and quickly find ways to feel at home in groups of strangers ',
        
      },
      {
        image: 'https://i.postimg.cc/XN5PtmhP/C11-Nozipho-Mayila-2.jpg',
        projectName: 'Nozipho Mayila',
        description: '',
        
      },
      
      {
        image: 'https://i.postimg.cc/Jzx6ZFzY/Lavish-Logo-Turquoise-Gold-an-Blue-Gradient.webp',
        projectName: '',
        description: 'Some people are naturally outgoing, conversational and quickly find ways to feel at home in groups of strangers. so i would say siwe is a people's person',
       
      ]
    }
  }
}
</script>

<style scoped>
.fade-enter-active,
.fade-leave-active {
  transition: all 0.9s ease;
  overflow: hidden;
  visibility: visible;
  position: absolute;
  width:100%;
  opacity: 1;
}

.fade-enter,
.fade-leave-to {
  visibility: hidden;
  width:100%;
  opacity: 0;
}

img {
  height:600px;
  width:100%
}

.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 40%;
  width: auto;
  padding: 16px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.7s ease;
  border-radius: 0 4px 4px 0;
  text-decoration: none;
  user-select: none;
}

.next {
  right: 0;
}

.prev {
  left: 0;
}

.prev:hover, .next:hover {
  background-color: rgba(0,0,0,0.9);
}
</style>



















