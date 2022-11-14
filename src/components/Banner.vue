<template>
   <div id="main-banner">
    <h1>Make Your Burger</h1>
    
   </div>
</template>

<script>
export default { name:"Banner"}


</script>

<style scoped>
#main-banner {
   background-image: url('/public/img/burger.jpg');
   height: 400px;   
   display:flex;
   
   align-items:flex-start;
   justify-content:center;
   background-position: center;
   background-size: cover;
   background-repeat: no-repeat;
   padding-top: 20px;
   
  
}
#main-banner h1 {
  color: #FFF;
   text-align:center;
   font-size: 50px;
   padding: 10px 5px;
   background-color:#222;
  

}

</style>
