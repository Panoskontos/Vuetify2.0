<template>
<div>
 <div>
    <div height="225px" class="row transparent mt-5 mx-10 d-flex justify-center" >

      
      <v-card 
       v-bind="props"
        :class="`elevation-${isHovering ? 24 : 6}`"
      height="225px" width="60%" class="row-card blue-grey darken-3 mr-10">

      <ConformityComponent/>

      </v-card>      
       
      
       
      <v-card 
       v-bind="props"
        :class="`elevation-${isHovering ? 24 : 6}`"
      height="225px" width="20%" class="row-card row-card-keys blue-grey darken-3 ">

      <KeysComponent/>

</v-card>
        
      
      
       
      <v-card 
       v-bind="props"
        :class="`elevation-${isHovering ? 24 : 6}`"
      height="225px" width="20%" class="row-card row-card-status blue-grey darken-3 ml-10">

  <StatusComponent/>

</v-card>
              

    </div>
    
    <div  height="200px" class="bg-transparent mx-10 mt-10 d-flex justify-center" > 
        
         
      <v-card 
       v-bind="props"
        :class="`elevation-${isHovering ? 24 : 6}`"
        
        height="230px" width="50%" class="blue-grey darken-3 mr-10">
        </v-card>      
          

     
      <v-card 
       v-bind="props"
        :class="`elevation-${isHovering ? 24 : 6}`"
         height="230px" width="50%" class="blue-grey darken-3 ">
        </v-card>

           
    
    </div>
    
      
    <v-card 
    v-bind="props"
        :class="`elevation-${isHovering ? 24 : 6}`"
    height="320px" class="blue-grey darken-3 mx-10 mt-10" 
     :style="{ 'background-color': hover ? 'red' : '#BB86FC' }"
    >      
    </v-card>
      

    </div>
</div>
</template>

<script>

  export default {
    name: 'HomeView',

    components: {
    },
  }
</script>

<style>
 @media only screen and (max-width: 1000px) { 
  .row {
    background-color: rgb(255, 255, 255);
    width: 80%;
    height: 750px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .row-card {
    width: 100% !important;
    margin-bottom: 20px;
    height: 205px !important;
    margin: auto !important;
  }
  .row-card-keys {
    /* height: 225px !important; */
  }
  .row-card-status {
    margin-right: 37px !important;
    /* height: 225px !important; */
  }
} 
</style>