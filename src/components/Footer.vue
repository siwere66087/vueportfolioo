<template>
   <div id="footer-container">
    <div id="footer">
      <div id="footer-contact">
        <p>{{ email }}</p>
        <p>{{ phone }}</p>
        <p>{{ socials }}</p>
      </div>
      <div id="footer-social">
       <div class="socials" ><a href=""><i class=" fab  fa-brands fa-facebook fa-2xl" ></i></a> </div>
        <div class="socials"> <a href=""><i class=" fab  fa-brands fa-twitter fa-2xl"></i></a></div>
        <div class="socials"><a href=""><i class=" fab  fa-brands fa-linkedin fa-2xl"></i></a></div>
        <div class="socials"><a href=""><i class=" fab  fa-brands fa-github fa-2xl"></i></a></div>
      </div>
    </div>
    <div id="copyright">
      <p>&copy;{{copyright }}</p>
    </div>
   </div>
</template>

<script>
    export default {
      data() {
        return {
            email:'sivuyisiwe.mgijima6@gmail.com',
            phone: '0683150682',
            copyright: 'copyright reserved developed by s.mgijima 2023'
        }
      },  
    }
</script>

<style scoped>


#footer-container{
  padding-top:20px;
  margin-top:20px;
  width:100vw;
  color:white;
  background-color:#1a1a1a;
  display:flex;
  flex-direction:column;
  align-items:center;
}
#footer{
  display:flex;
  justify-content:space-around;
  align-items:center;
  width:100%;
}
#footer-contact{
  text-align:right;
}
#footer-social{
  width:20%;
  display : flex;
  justify-content : space-between;
}
.socials a i {

width: 50px;
height: 50px;
border-radius: 50%;
/* background-color: #fff; */

}


#footer-social div i{
  height:50px ;
  width:50px;
  padding-top: 15px;

  border-radius:50%;
}
#address p {
  font-size:0.5em;
}




#copyright{
    margin-right: 45rem;
}
</style>