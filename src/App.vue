<template>
  <v-app>
    <v-app-bar
      app
      dark
      
    >
   <v-app-bar
    flat
    dense
    :max-width="1000"
    style="margin:auto"

   >
   <v-icon class="blue--text">mdi-map-marker</v-icon>
   <v-icon>mdi-menu-down</v-icon>
      <v-toolbar-title>Manila, Philippines</v-toolbar-title>   
       <v-spacer> </v-spacer> 
        <v-btn text class="">
       <span>Sign in</span>
      </v-btn>

      <v-btn text>
        Registers
      </v-btn>

     
   </v-app-bar>
    </v-app-bar>

    <v-main>
        <Home />
    </v-main>
  </v-app>
</template>

<script>
//import HelloWorld from './components/HelloWorld';
import Home from './views/Home'
export default {
  name: 'App',

  components: {
    //HelloWorld,
    Home,
  },

  data: () => ({
    //
  }),
};
</script>
