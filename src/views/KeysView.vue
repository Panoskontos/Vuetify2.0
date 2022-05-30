<template>
<div>
 <div>
    <div class="row transparent white--text mt-5 mx-10 d-flex justify-start" >
      
<v-card

    dark
>
    <v-card-title>
      Keys
      <v-spacer></v-spacer>
      <v-text-field
        v-model="search"
        append-icon="mdi-magnify"
        label="Search"
        single-line
        hide-details
      ></v-text-field>
    </v-card-title>
    <v-data-table
      :headers="headers"
      :items="minions"
      :search="search"
>
<!-- Conformity Buttons -->
<template v-slot:item.status="{ item }">
      <v-chip
        class="success"
        dark
      >
        {{ item.status }} 
      </v-chip>
</template>

<!-- Fix the table -->

<!-- Actions -->
<template v-slot:item.actions="{ item }">
<v-btn
  class="primary mr-3 rounded-lg"
    @click="editItem(item)"
>
    Reject
</v-btn>


<v-btn
  class="red mr-3 rounded-lg"

    @click="editItem(item)"
>
    Deny
</v-btn>
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
          { text: 'Status', value: 'status' },
          { text: 'Public Key', value: 'public_key' },
          { text: 'Actions', value: 'actions' },
        ],
        minions: [
          {
            jid: '3d4fs843hfiwer',
            status: 'Accepted',
            public_key: 'fb21343djsgfjwe45345fejef',
            actions: ''
          },
          {
            jid: '3d4fs843hfiwer',
            status: 'Accepted',
            public_key: 'fb21343djsgfjwe45345fejef',
            actions: ''
          },
      ]
      }
    }
  }

</script>