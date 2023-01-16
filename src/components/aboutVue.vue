<template>
   <div id="about" class="about">
      <div class="container" v-for="item in about" :key="item">
        <div class="row justify-content-between">

          <div class="col-lg-4 ">
            <div class="div-img-bg">
              <div class="about-img">
                <img :src="item.image" class="img">
              </div>
            </div>
          </div>

          <div class="col-lg-7">
            <div class="about-descr">

              <p class="p-heading">{{ item.description }} </p>
              
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
#about {
  width: 100%;
  height: auto;
  background: #f7f7f7;
  padding-top: 120px;
  position: fixed;
}

#about .div-img-bg {
  padding-bottom: 30px;
  border: 20px solid #eb410d;
}

#about .div-img-bg .about-img img {
  width: 100%;
  box-shadow: 0px 0px 85px 0px rgba(0, 0, 0, 0.14);
  margin-top: -60px;
  margin-left: 40px;
  height: 400px;
  object-fit: cover;
}

#about .about-descr .p-heading {
  font-family: "Playfair Display", serif;
  font-size: 28px;
  text-align: left;
}

#about .about-descr  {
  max-width: 80%;
  margin-bottom: 0;
  text-align: left;
}
.head-info .header-content  {
    font-size: 32px;
  }

  #about .div-img-bg {
    padding: 0;
  }

  #about .div-img-bg .about-img img {
    margin-top: 0%;
    margin-left: calc(0% - 0px);
  }

  #about .about-descr .p-heading {
    font-size: 20px;
  }

  #about .about-descr  {
    max-width: 100%;
    margin-bottom: 0;
  }


/* media query */
@media (max-width: 320px) {

/* Navbar */
nav {
  padding: 20px 15px;
}

.nav-menu {
  margin-top: 40px;
  display: none;
  float: none;
  width: 100%;
}

.nav-menu li {
  float: none;
  width: 100%;
  text-align: center;
  border-top: 1px solid #f7f7f7;
  line-height: 45px;
  margin-left: 0;
  padding-top: 10px;
  padding-bottom: 10px;
}

.responsive {
  float: right;
  padding-top: 15px;
  display: block;
}

/* About */
.head-info .header-content h1 {
  font-size: 32px;
}

#about .div-img-bg {
  padding: 0;
}

#about .div-img-bg .about-img img {
  margin-top: 0%;
  margin-left: calc(0% - 0px);
}

#about .about-descr .p-heading {
  font-size: 20px;
}

#about .about-descr  {
  max-width: 100%;
  margin-bottom: 0;
}

}
/** Width between 480px to 0

 */
 @media (max-width: 480px) {

/* Navbar */
nav {
  padding: 20px 15px;
}

.nav-menu {
  margin-top: 40px;
  display: none;
  float: none;
  width: 100%;
}

.nav-menu li {
  float: none;
  width: 100%;
  text-align: center;
  border-top: 1px solid #f7f7f7;
  line-height: 45px;
  margin-left: 0;
  padding-top: 10px;
  padding-bottom: 10px;
}



/* About */
.head-info .header-content h1 {
  font-size: 32px;
}

#about .div-img-bg {
  padding: 0;
}

#about .div-img-bg .about-img img {
  margin-top: 0%;
  margin-left: calc(0% - 0px);
}

#about .about-descr .p-heading {
  font-size: 20px;
}

#about .about-descr  {
  max-width: 100%;
  margin-bottom: 0;
}

}

/** Width between 600px to 0

 */
 @media (max-width: 600px) {

/* Navbar */
nav {
  padding: 20px 15px;
}

.nav-menu {
  margin-top: 40px;
  display: none;
  float: none;
  width: 100%;
}

.nav-menu li {
  float: none;
  width: 100%;
  text-align: center;
  border-top: 1px solid #f7f7f7;
  line-height: 45px;
  margin-left: 0;
  padding-top: 10px;
  padding-bottom: 10px;
}

.responsive {
  float: right;
  padding-top: 15px;
  display: block;
}

/* About */
.head-info .header-content h1 {
  font-size: 32px;
}

#about .div-img-bg {
  padding: 0;
}

#about .div-img-bg .about-img img {
  margin-top: 0%;
  margin-left: calc(0% - 0px);
}

#about .about-descr .p-heading {
  font-size: 20px;
}

#about .about-descr {
  max-width: 100%;
  margin-bottom: 0;
}

}


/** Width between 767px to 0
 *  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 */
 @media (max-width: 767px) {

/* Navbar */
nav {
  padding: 20px 15px;
}

.nav-menu {
  margin-top: 40px;
  display: none;
  float: none;
  width: 100%;
}

.nav-menu li {
  float: none;
  width: 100%;
  text-align: center;
  border-top: 1px solid #f7f7f7;
  line-height: 45px;
  margin-left: 0;
  padding-top: 10px;
  padding-bottom: 10px;
}

.responsive {
  float: right;
  padding-top: 15px;
  display: block;
}

/* About */
.head-info .header-content h1 {
  font-size: 32px;
}

#about .div-img-bg {
  padding: 0;
}

#about .div-img-bg .about-img img {
  margin-top: 0%;
  margin-left: calc(0% - 0px);
}

#about .about-descr .p-heading {
  font-size: 20px;
}

#about .about-descr{
  max-width: 100%;
  margin-bottom: 0;
}
}

@media (min-width: 768px) and (max-width: 991px) {

/* Navbar */
nav {
  padding: 10px 15px;
}

.nav-menu {
  margin-top: 40px;
  display: none;
  float: none;
  width: 100%;
}

.nav-menu li {
  float: none;
  width: 100%;
  text-align: center;
  border-top: 1px solid #f7f7f7;
  line-height: 45px;
  margin-left: 0;
  padding-top: 10px;
  padding-bottom: 10px;
}

.responsive {
  float: right;
  padding-top: 15px;
  display: block;
}

/* About */
.head-info .header-content  {
  font-size: 32px;
}

#about .div-img-bg {
  padding: 0;
}

#about .div-img-bg .about-img img {
  margin-top: 0%;
  margin-left: calc(0% - 0px);
}

#about .about-descr .p-heading {
  font-size: 20px;
}

#about .about-descr {
  max-width: 100%;
  margin-bottom: 0;
}
}

</style>
