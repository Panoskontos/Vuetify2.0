<template>
<div>
 <div>
    <div class="row transparent white--text mt-5 mx-10 d-flex justify-start" >
      
      <v-card dark width="100%" class="row-card px-10">
     <v-card-title>
      <v-text-field
        v-model="search"
        append-icon="mdi-magnify"
        label="Search"
        single-line
        hide-details
      ></v-text-field>
    </v-card-title>
    <v-data-table
      class="blue-grey darken-3 elevation-1 white--text"
      :headers="headers"
      :items="minions"
      :search="search"
    >

<template v-slot:item.Conformity="{ item }">
      <v-chip
        class="green"
        dark
      >
        {{ item.Conformity }} 
      </v-chip>
</template>


    </v-data-table>
     
     </v-card>      
              

    </div>
    
    
    
    </div>
</div>
</template>

<script>
// import ButtonComponent from '../components/ButtonComponent.vue'


  export default {
    name: 'MinionsView',
    conponents:{
      // ButtonComponent
      },
    data () {
      return {
        search: '',
        headers: [
          {
            text: 'Minion Id',
            align: 'start',
            value: 'jid',
          },
          { text: 'Conformity', value: 'Conformity' },
          { text: 'F.Q.D.N', value: 'FQDN' },
          { text: 'O.S', value: 'OS' },
          { text: 'O.S. Version', value: 'OSVersion' },
          { text: 'Kernel', value: 'Kernel' },
          { text: 'Last Job', value: 'l_job' },
          { text: 'Last Highstate', value: 'l_highstate' },
          { text: 'Actions', value: '' },
        ],
        minions: [
          {
            jid: '3d4fs843hfiwer',
            Conformity: 'True',
            FQDN: '3d4fs843hfiwer',
            OS: 'Debian',
            OSVersion: 'strech',
            Kernel: '5.2.17-200.fc30.x86_64',
            l_job: '09/10/2019 08:09:55',
            l_highstate: '',
          },
          {
            jid: 'as234dasd34sf',
            Conformity: 'True',
            FQDN: 'as234dasd34sf',
            OS: 'Debian',
            OSVersion: 'strech',
            Kernel: '5.2.17-200.fc30.x86_64',
            l_job: '27/10/2022 08:09:55',
            l_highstate: '',
          },
          {
            jid: '923dsf4s843hf',
            Conformity: 'True',
            FQDN: '923dsf4s843hf',
            OS: 'Windows',
            OSVersion: '11',
            Kernel: '5.2.17-200.fc30.x86_64',
            l_job: '1/10/2021 09:09:55',
            l_highstate: '',
          },
         
          
        ],
      }
    }
  }
</script>

<style scoped>
.row-card{
  background-color: #1e1e24;  
}


 @media only screen and (max-width: 1000px) { 
  
  body {
    background-color: black;
  }
  
  .row {
    width: 88%;
  }

  .row-card {
  background-color: #1e1e24;

   position: absolute;
   top: 20px;
  }
} 
</style>