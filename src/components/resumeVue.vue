<template>
 <section id="resume" style="background-color: white;" >
		<div class="container">
			<div class="row">
				<div class="col-md-12 col-md-offset-0">
					<ul class="resumeInfo" v-for="item in resume" :key="item">
						<li class="resumeInfo-heading text-center ">
							<div><h3>Work Experience</h3></div>
						</li>

						<li class="animate-box resumeInfo-unverted">
							<div class="resumeInfo-icon"><i class="fa-solid fa-graduation-cap"></i></div>
							<div class="resumeInfo-panel">
								<div class="resumeInfo-heading">
									<h3 class="resumeInfo-title">{{ item.title }}</h3>
									<span class="company">{{ item.place }} </span>
								</div>
								<div class="resumeInfo-body">
                                    <h5 class="duties">duties</h5>
									<p> {{ item.description }}</p>
								</div>
							</div>
						</li>
                    </ul>
				</div>
			</div>
		</div>
   </section>
	

</template>

<script>

    export default {
        
        data() {
            return {
                name:'resume',
                resume:[
                {title:'high school',
                place:'Kwamfundo high school 2015',
                description:'matriculant'
                
               
             },
                {title:'Teacher Assistant',
                place:'Manyano high school - 2019 july - December',
                description:'getting the classroom ready for lessons.,helping children who need extra support to complete tasks'
                
               
             },
             {title:'sales ',
                place:'Brights - 2021 march - july',
                description:'Ensure high levels of customer satisfaction through excellent sales service.Recommend and display items that match customer needs.'
                
               
            },
            {title:'Teacher Assistant',
                place:'Esangweni high school - 2021 july - December',
                description:'getting the classroom ready for lessons.,helping children who need extra support to complete tasks'
                
               
            },
            {title:'front end developer',
                place:'Life choices - 2021 september - 2022 December',
                description:'web development'
                
               
            },

                ]
            }
        }



    }
</script>

<style  scoped>
.duties{

color: #010101;
font-size: 23px;
text-transform: capitalize;

}

.resumeInfo {
  list-style: none;
  padding: 20px 0 20px;
  position: relative;
}
.resumeInfo:before {
  top: 20px;
  bottom: 0;
  position: absolute;
  content: " ";
  width: 2px;
  background-color: #e6e6e6;
  left: 50%;
  margin-left: 0px;
}
@media screen and (max-width: 768px) {
  .resumeInfo:before {
    margin-left: -64px;
  }
}
@media screen and (max-width: 480px) {
  .resumeInfo:before {
    margin-left: -64px;
  }
}
@media screen and (max-width: 768px) {
  .resumeInfo .resumeInfo-heading {
    margin-bottom: 30px;
  }
}
.resumeInfo .resumeInfo-heading  div h3 {
  display: inline-block;
  padding: 7px 15px;
  font-size: 18px;
  text-transform: uppercase;
  font-weight: bold;
  background: #e6e6e6;
  border-radius: 4px;
}
@media screen and (max-width: 768px) {
  .resumeInfo .resumeInfo-heading  div h3 {
    float: left;
    margin-bottom: 0;
  }
}
.resumeInfo  li {
  margin-bottom: 20px;
  position: relative;
}
@media screen and (max-width: 768px) {
  .resumeInfo  li {
    margin-bottom: 4em;
  }
}
.resumeInfo  li:before, .resumeInfo  li:after {
  content: " ";
  display: table;
}
.resumeInfo  li:after {
  clear: both;
}
.resumeInfo  li  .resumeInfo-panel {
  width: 45%;
  float: left;
  margin-bottom: 0;
  position: relative;
  border-radius: 4px;
}
@media screen and (max-width: 768px) {
  .resumeInfo  li  .resumeInfo-panel {
    width: 85% !important;
  }
}
@media screen and (max-width: 480px) {
  .resumeInfo  li  .resumeInfo-panel {
    width: 75% !important;
  }
  .resumeInfo  li  .resumeInfo-panel:before {
    top: 30px;
  }
  .resumeInfo  li 
  .resumeInfo-panel:after {
    top: 31px;
  }
}
.resumeInfo li  .resumeInfo-icon {
  color: #fff;
  width: 44px;
  height: 44px;
  line-height: 50px;
  font-size: 1.4em;
  text-align: center;
  position: absolute;
  top: 40px;
  left: 50%;
  margin-left: -21px;
  background-color: #ff0000;
  z-index: 100;
  display: table;
 
  border-radius: 50%;
}
@media screen and (max-width: 768px) {
  .resumeInfo > li > .resumeInfo-badge {
    margin-left: -10px !important;
  }
}
@media screen and (max-width: 992px) {
  .resumeInfo  li  .resumeInfo-badge {
    margin-left: -10px !important;
  }
}
.resumeInfo li  .resumeInfo-badge i {
  display: table-cell;
  vertical-align: middle;
  height: 44px;
  font-size: 18px;
}
.resumeInfo  li.resumeInfo-unverted {
  text-align: right;
}
@media screen and (max-width: 768px) {
  .resumeInfo  li.resumeInfo-unverted {
    text-align: left;
  }
}
.resumeInfo  li.resumeInfo-inverted .resumeInfo-panel {
  float: right;
}
.resumeInfo  li.resumeInfo-inverted  .resumeInfo-panel:before {
  border-left-width: 0;
  border-right-width: 15px;
  left: -15px;
  right: auto;
}
.resumeInfo  li.resumeInfo-inverted  .resumeInfo-panel:after {
  border-left-width: 0;
  border-right-width: 14px;
  left: -14px;
  right: auto;
}

.resumeInfo-title {
  margin-top: 0;
}

.company {
  display: block;
  margin-bottom: 20px;
  font-size: 18px;
  font-weight: 600;
  color: #181818;
}

.resumeInfo-body  ,
.resumeInfo-body  ul {
  margin-bottom: 0;
  color: #010101;
}

.resumeInfo-body  p {
  margin-top: 5px;
  color: #010101;
}

@media (max-width: 992px) {
  ul.resumeInfo:before {
    left: 90px;
  }

  ul.resumeInfo  li  .resumeInfo-panel {
    width: calc(100% - 200px);
    width: -moz-calc(100% - 200px);
    width: -webkit-calc(100% - 200px);
  }

  ul.resumeInfo  li  .resumeInfo-badge {
    left: 15px;
    margin-left: 0;
    top: 16px;
  }

  ul.resumeInfo  li  .resumeInfo-panel {
    float: right;
  }

  ul.resumeInfo  li  .resumeInfo-panel:before {
    border-left-width: 0;
    border-right-width: 15px;
    left: -15px;
    right: auto;
  }

  ul.resumeInfo  li  .resumeInfo-panel:after {
    border-left-width: 0;
    border-right-width: 14px;
    left: -14px;
    right: auto;
  }
}

</style>