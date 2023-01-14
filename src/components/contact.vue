
<template>
    
    <div class="row" style="background-color: white;">

    <div class="content">

   <div class="info"  v-for="item in info" :key="item" >

    <h3> <i class="fas fa-envelope"></i> {{item.myemail }} </h3>
    <h3> <i class="fas fa-phone"></i> {{ item.phone }}</h3>
    <h3> <i class="fas fa-map-marker-alt"></i> {{ item.address }} </h3>
    </div>

    </div>


    <Form method="post"  action="https://formspree.io/f/xoqbpgvr"  v-model="values"
      @submit="handlesubmit"
    >
        <input type="text"  name="name" placeholder="name" class="box" required>
        <input type="text" name="email" class="box" placeholder="enter your email" required />
        <textarea name="" id="" cols="20" rows="5" class="box" placeholder="message" required></textarea>

      <input type="submit" label="submit" />
      <div></div>
    </Form>
</div>
  </template>
  
  <script>
  export default {
    
    
    data () {
         return { values: {},
         info:[],
         handlesubmit: () => alert('submitted successfully')
        
        }},

       mounted() {
        this.info = [{
        myemail:'siwe@gmail.com',
        phone:'0683150682',
        address:'South Africa, western cape, cape town, 7784'


        }]
       },
    
    
    }
  </script>
  
<style scoped>

.content{
    flex:1 1 30rem;
    padding:4rem;
    padding-bottom: 0;
}
.content .info h3{
    display: flex;
    align-items: center;
    font-size: 2rem;
    color:rgb(6, 6, 6);
    padding:1rem 0;
    font-weight: normal;
}
.content .info h3 i{
    padding-right: 1rem;
    color:var(--yellow);
}
form{
    flex:1 1 45rem;
    padding:2rem;
    margin:2rem;
    margin-bottom: 4rem;
    border: 2px solid black;
}
form .box{
    padding:1.5rem;
    margin:1rem 0;
    background:#3333;
    color:#fff;
    text-transform: none;
    font-size: 1.7rem;
    width:100%;
}
.row form .message{
    height: 15rem;
    resize: none;
}
.row .content .info .title{
    text-transform: uppercase;
    color:#fff;
    font-size: 3rem;
    padding-bottom: 2rem;
}
.row .content .info h3 i{
    padding-right: 1rem;
    color:rgb(195, 59, 149);
}

</style>






