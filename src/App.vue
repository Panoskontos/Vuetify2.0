<template>
  <v-app>
    <div class="body">
    <!-- Toolbar -->
     <v-app-bar class="flex-grow-0 appbar" app dark>
    
    
    <v-app-bar-title></v-app-bar-title>

      <v-spacer></v-spacer>
        
              <v-btn icon>
                <v-icon>mdi-magnify</v-icon>
              </v-btn>

      <v-btn icon>
        <v-badge
        color="red"
          dot
          overlap
                  >

              <v-icon>mdi-bell</v-icon>
          </v-badge>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>


   </v-app-bar>

    <!-- Navbar -->
      <v-navigation-drawer app v-model="drawer"
      expand-on-hover
      dark
      permanent
      width="250px"
      height="100vh"
      class="rounded-md blue-grey darken-4 sidenav"
      >
<!-- empty item -->
      <!-- <v-list-item class="mt-2">
        <v-list-item-content>
          <v-list-item-title class="text-h6"> 
            
            </v-list-item-title>
        </v-list-item-content>
</v-list-item> -->

<!--  -->
        <!-- <v-divider></v-divider> -->
        <v-list>
          <v-list-item class="px-2 pt-4  d-flex justify-center">
            <v-list-item-avatar class="grey darken-4 ">
              <v-img src="https://lh3.googleusercontent.com/-4_ZEHFWjQ10/AAAAAAAAAAI/AAAAAAAAAAA/C8YPLHf4HqQ/s55-p-k-no-ns-nd/photo.jpg"></v-img>
            </v-list-item-avatar>
          </v-list-item>

<br>
            <v-divider></v-divider>


          <v-list-item class="px-2 pt-1  d-flex justify-space-around" link>
            <v-list-item-avatar>
              <v-img src="https://randomuser.me/api/portraits/men/90.jpg"></v-img>
            </v-list-item-avatar>
            <v-list-item-content>

              <v-list-item-title class="text-h8">
                Panos Kontos
              </v-list-item-title>
<v-list-item-subtitle>panos@gmail.com</v-list-item-subtitle>
            </v-list-item-content>

          </v-list-item>

            <v-divider></v-divider>

          
      

          <!-- <v-list-item link>
            <v-list-item-content>
              <v-list-item-title class="text-h8">
                Panos Kontos
              </v-list-item-title>
              <v-list-item-subtitle>panos@gmail.com</v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item> -->
        </v-list>

        <!-- <v-divider></v-divider> -->

        <v-list
          nav
          dense
        >

<!-- Icons https://icon-sets.iconify.design/mdi/ -->

 <router-link to="/">
        <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item>
  </router-link >

<router-link to="/about">
      <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-vector-point</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Minions</v-list-item-title>
          </v-list-item>
</router-link>
          
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-key-chain</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Keys</v-list-item-title>
          </v-list-item>

          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-play</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Jobs</v-list-item-title>
          </v-list-item>

          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-account-multiple</v-icon>
            </v-list-item-icon>
            <v-list-item-title>About</v-list-item-title>
          </v-list-item>
      
        </v-list>
      </v-navigation-drawer>

      <v-main >
        
          <router-view/>
        </v-main>
     
       
     


  </div>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => {
      return {
         drawer: true,
        }
     }
};
</script>

<style scoped>
a {
    text-decoration: none !important;
}


#app{
  background-color: #1e1e24;
}


.appbar {
  background-color: #1e1e24 !important;

}

</style>