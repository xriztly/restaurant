<template>
  <div class="home">
   <br>
   <br>
   <div id="test">
     <div id="image-sectio">
        <v-img
          class="rounded-xl"
        height="300"
         width="100%"
        src="https://picsum.photos/id/11/500/300"
    >
  <form class="rounded-pill" >
    
  <div  class="justify-center d-flex justify-center " style="margin:200px;">
    <!-- Input -->
    <input type="search"  placeholder="Search resto">
    <!-- Clear button -->
   <input type="submit" value="Search">
    
  </div>

</form>
</v-img>
 
 
     </div>

  <br />
  <p>Not in 
    <span style="font-weight:bold">Manila</span> ? Get current location here!
    <span><a id="a" href="#"><v-icon class="blue--text">mdi-compass-outline</v-icon></a></span>
    </p>

<br> <br>

<!--Dinner Suggestion Section--->
  <v-flex>
    <div >
     <div class="d-inline" style="font-weight:bold"> Dinner Suggestions</div>
     <div class="d-inline float-right"> <a id="a" href="#">View all</a> </div>
    </div>

     <v-item-group mandatory>
    <v-container>
      <v-row>
        <v-col
          v-for="n in itemdinner"
          :key="n"
          xl="6"
          
        >
          <v-item >
             <v-card
 
   >
   <div style="margin:auto;">
    <v-img style="margin:auto"
    class="rounded-lg"
      height="150"
      width="140"
      src="https://cdn.vuetifyjs.com/images/cards/cooking.png"
    ></v-img>

   </div>
   
    <v-card-title>{{n.name}}</v-card-title>

    <div>
      <div class="d-inline-block">
           <v-icon class="blue--text">mdi-map-marker</v-icon>
      </div>
      <div class="d-inline-block ">
       <p>$ • {{n.restoName}}</p>
      </div>
    </div>
    <v-card-text>
      <v-row
        align="center"
        class="mx-0"
      >
        <v-rating
          :value="1"
          color="amber"
          dense
           :length="1"
          size="20"
        ></v-rating>
        <div class="grey--text">
         {{ n.ratings}}
        </div>
        
        <div class="grey--text ml-12">
          {{n.loc}}
        </div>
      </v-row>

       </v-card-text>

   
   
      </v-card>
              </v-item>
            </v-col>
          </v-row>
        </v-container>
      </v-item-group>

   </v-flex>

 <br>
 <br>

<!--Jus For You Section--->
<v-flex>
    <div >
     <div class="d-inline" style="font-weight:bold">Just For You!</div>
     <div class="d-inline float-right"> <a id="a" href="#">View all</a> </div>
    </div>

     <v-item-group mandatory>
    <v-container>
      <v-row>
        <v-col
          v-for="n in 6"
          :key="n"
          xl="6"
        >
          <v-item >
             <v-card
 
   >
   <div style="margin:auto;">
    <v-img style="margin:auto"
    class="rounded-lg"
      height="150"
      width="140"
      src="https://cdn.vuetifyjs.com/images/cards/cooking.png"
    ></v-img>

   </div>
   
    <v-card-title>Cafe Badilico</v-card-title>

    <div>
      <div class="d-inline-block">
           <v-icon class="blue--text">mdi-map-marker</v-icon>
      </div>
      <div class="d-inline-block ">
       <p>$ • Italian, Cafes</p>
      </div>
    </div>
    <v-card-text>
      <v-row
        align="center"
        class="mx-0"
      >
        <v-rating
          :value="1"
          color="amber"
          dense
           :length="1"
          size="20"
        ></v-rating>
        <div class="grey--text">
          4.5
        </div>
        
        <div class="grey--text ml-12">
          Asia
        </div>
      </v-row>

       </v-card-text>

   
   
      </v-card>
              </v-item>
            </v-col>
          </v-row>
        </v-container>
      </v-item-group>

   </v-flex>

   <br>
  <br>

  <!--Popular restaurants Section--->
  <v-flex>
    <div >
     <div class="d-inline" style="font-weight:bold">Popular restaurants</div>
     <div class="d-inline float-right"> <a id="a" href="#">View all</a> </div>
    </div>

     <v-item-group mandatory>
    <v-container>
      <v-row>
        <v-col
          v-for="n in 6"
          :key="n"
          xl="6"
        >
          <v-item >
             <v-card
 
   >
   <div style="margin:auto;">
    <v-img style="margin:auto"
    class="rounded-lg"
      height="150"
      width="140"
      src="https://cdn.vuetifyjs.com/images/cards/cooking.png"
    ></v-img>

   </div>
   
    <v-card-title>Cafe Badilico</v-card-title>

    <div>
      <div class="d-inline-block">
           <v-icon class="blue--text">mdi-map-marker</v-icon>
      </div>
      <div class="d-inline-block ">
       <p>$ • Italian, Cafes</p>
      </div>
    </div>
    <v-card-text>
      <v-row
        align="center"
        class="mx-0"
      >
        <v-rating
          :value="1"
          color="amber"
          dense
           :length="1"
          size="20"
        ></v-rating>
        <div class="grey--text">
          4.5
        </div>
        
        <div class="grey--text ml-12">
          Asia
        </div>
      </v-row>

       </v-card-text>

   
   
      </v-card>
              </v-item>
            </v-col>
          </v-row>
        </v-container>
      </v-item-group>

   </v-flex>
   <br>
    <br>

  <!--Restaurants Near you Section--->
   <v-flex>
    <div >
     <div class="d-inline" style="font-weight:bold">Restaurants Near you</div>
     <div class="d-inline float-right"> <a id="a" href="#">View all</a> </div>
    </div>

     <v-item-group mandatory>
    <v-container>
      <v-row>
        <v-col
          v-for="n in 6"
          :key="n"
          xl="6"
        >
          <v-item >
             <v-card
 
   >
   <div style="margin:auto;">
    <v-img style="margin:auto"
    class="rounded-lg"
      height="150"
      width="140"
      src="https://cdn.vuetifyjs.com/images/cards/cooking.png"
    ></v-img>

   </div>
   
    <v-card-title>Cafe Badilico</v-card-title>

    <div>
      <div class="d-inline-block">
           <v-icon class="blue--text">mdi-map-marker</v-icon>
      </div>
      <div class="d-inline-block ">
       <p>$ • Italian, Cafes</p>
      </div>
    </div>
    <v-card-text>
      <v-row
        align="center"
        class="mx-0"
      >
        <v-rating
          :value="1"
          color="amber"
          dense
           :length="1"
          size="20"
        ></v-rating>
        <div class="grey--text">
          4.5
        </div>
        
        <div class="grey--text ml-12">
          Asia
        </div>
      </v-row>

       </v-card-text>

   
   
      </v-card>
              </v-item>
            </v-col>
          </v-row>
        </v-container>
      </v-item-group>

   </v-flex>

   </div>
  </div>
  
  </template>

<script>
export default {
  data (){

    return{
      itemdinner:[
        { name: 'Cafe Badilico', src: '../assets/logo.png', restoName: 'Italian, Cafe', ratings: '4.5', loc: 'Asia'},
           { name: 'Cafe Badilico', src: '../assets/logo.png', restoName: 'Italian, Cafe', ratings: '4.5', loc: 'Asia'},
            { name: 'Cafe Badilico', src: '../assets/logo.png', restoName: 'Italian, Cafe', ratings: '4.5', loc: 'Asia'},
             { name: 'Cafe Badilico', src: '../assets/logo.png', restoName: 'Italian, Cafe', ratings: '4.5', loc: 'Asia'},
              { name: 'Cafe Badilico', src: '../assets/logo.png', restoName: 'Italian, Cafe', ratings: '4.5', loc: 'Asia'},
               { name: 'Cafe Badilico', src: '../assets/logo.png', restoName: 'Italian, Cafe', ratings: '4.5', loc: 'Asia'},
      ]
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

input[type=search] {
  width: 500px;
  padding: 12px 20px;
  margin: 8px 0;
  background-color: cornsilk;
  outline: none;

}

input[type=submit] {
  background-color: royalblue;
  color: cornsilk;
  padding: 12px 20px;
  margin: 8px 0;
  
}

#a{
  text-decoration: none;
}
</style>