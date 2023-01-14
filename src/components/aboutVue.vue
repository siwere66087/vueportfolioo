<template>
  <section id="about" class="section wb">
        <div class="container">
            <div class="row"  v-for="item in about" :key="item">
                <div class="col-md-6">
                    <div class="message-box">                        
                        <h2 class="name">Sivuyisiwe Mgijima</h2>
                        <p class="abtD"> {{ item.description }} </p>
						       </div>
                </div>

                <div class="col-md-6">
                    <div class="right-box-pro wow fadeIn">
                      <img :src="item.image" class="img">
                    </div>
                </div>

				<div id="social-icons">
  <li><a href="" id="icons"><i class="  fa-brands fa-facebook"></i> </a></li>
  <li><a href="" id="icons"><i class="fa-brands fa-twitter"></i> </a></li>
  <li><a href="" id="icons"><i class="fa-brands fa-linkedin"></i> </a></li>
  <li><a href="" id="icons"><i class="fa-brands fa-instagram"></i> </a></li>
 
 </div>



            </div>
        </div>
  </section>
	
</template>

<script>
    export default {
        data() {
            return {
                name:'about',
                about:[{
                    image:'https://i.postimg.cc/jSJccHYP/IMG-20221019-WA0017.jpg',
                    description:'im a positive individual with great communication skills.I work efficiently as an individual as well as along with a team. I believe in character, values, vision, and action. I am a quick learner and believe in learning from my mistakes for I strongly feel that this virtue will take me ahead in life and career'



                }]
            }
        },
    }
</script>

<style scoped>
.name{
color: rgb(193, 33, 33);
font-size: 23px;

}

.abtD{
	color: white;
}
#social-icons{
width: 550pxx;
display: flex;
padding-bottom: 20rem;
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