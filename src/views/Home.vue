<template>
  <div class="home">
   <br>
   <br>
   <div id="test">
<v-img
  class="rounded-xl"
 height="300"
  width="100%"
  src="https://picsum.photos/id/11/500/300"
>
 
 
</v-img>
  <br />
  <p>Not in 
    <span style="font-weight:bold">Manila</span> ? Get current location here!
    </p><v-btn><v-icon class="blue--text">mdi-compass-outline</v-icon> </v-btn>
   </div>
     
  </div>
  
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
   
  }, data(){
    return {
        items: [
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
          },
         
           
        ],
      }
  }
}
</script>


<style scoped>

#test{
  margin:auto; 
  width:80%;
  max-height:auto;
 

}
</style>