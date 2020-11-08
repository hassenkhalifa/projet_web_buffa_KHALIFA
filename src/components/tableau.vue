<template>

  <md-table md-card>
    <md-table-toolbar>
      <h1 class="md-title">Restaurants</h1>
    </md-table-toolbar>

    <md-table-row>
      <md-table-head>Nom</md-table-head>
      <md-table-head>Cuisine</md-table-head>
    </md-table-row>

    <md-table-row v-for="(restaurant, index) in restaurants" :key="index" 
                @click="supprimerRestaurant(r)" 
                :style="{backgroundColor:getColor(index)}"
                :class="{bordureRouge:(index === 2)}">
      <md-table-cell>{{r.name}}</md-table-cell>
      <md-table-cell>{{r.cuisine}}</md-table-cell>
    </md-table-row>
  </md-table>
</template>


}

<script>
      
export default {
  name: "TableCard",

}

  
</script>