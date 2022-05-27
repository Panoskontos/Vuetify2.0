<template>
<div>
    <div class="px-10 pt-5 d-flex grey--text text--lighten-1 justify-start">
        <h3>Conformity</h3>
    </div>
    <!-- row -->
    <div class=" px-10 mt-6 d-flex justify-space-between align-center">
        <div class="grey--text text--lighten-1">
            HIGHSTATE
        </div>
        <v-card width="80%" height="16px" class="rounded-0 bg-transparent ">
            <LinearChart/>
        </v-card>
    </div>
    <!-- row -->
    <div class="px-10 mt-5 d-flex justify-space-between align-center">
        <div class="grey--text text--lighten-1">
            PYVERSION
        </div>
        <v-card width="80%" height="16px" class="rounded-0 bg-transparent ">
            <div class="green darken-1">
    <v-progress-linear
      background-color="green lighten-1"
      color="green lighten-4"
      height="18"
      value="45"
      buffer-value="65"
    >
    
   
    </v-progress-linear>
    </div>
        </v-card>
    </div>
    <!-- row -->
    <div class="px-10 mt-5 d-flex justify-space-between align-center">
        <div class="grey--text text--lighten-1" style="width:97px">
        FOO
        </div>
        <v-card width="80%" height="16px" class="rounded-0 bg-transparent ">
        
            <div class="blue darken-3">
    <v-progress-linear
      background-color="blue"
      color="blue lighten-3"
      height="18"
      value="23"
      buffer-value="60"
    >
    
    
    </v-progress-linear>
    </div>
        </v-card>
    </div>

</div>
</template>


<script>
import LinearChart from './LinearChart.vue'

export default {
    components:{
        LinearChart
    }
    
}
</script>

<style>


</style>