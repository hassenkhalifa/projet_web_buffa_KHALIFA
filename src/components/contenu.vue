<template>


  <md-content md-theme="selection-black">
    <h1>Nombre de restaurants : {{ nbRestaurantsTotal }}</h1>
    <p>Ajouter un restaurant</p>
    <md-field @input="chercherRestaurants()">
      <label>nom :</label>
      <md-input       
       type="text" required v-model="nom"
      ></md-input>
        </md-field>
      <md-field @input="chercherRestaurants()">
      <label>cuisine :</label>
      <md-input       
        type="text" required v-model="cuisine"
      ></md-input>
    </md-field>
    <md-field>
      <label>Chercher par nom :</label>
      <md-input
        @input="chercherRestaurants()"
        type="text"
        v-model="nomRestauRecherche"
      ></md-input>
    </md-field>
    
    <p>Nb de pages total : {{ nbPagesTotal }}</p>
    <md-button
      class="md-raised md-primary"
      :disabled="page === 0"
      @click="pagePrecedente()"
      >Précédent</md-button
    >
    <md-button
      class="md-raised md-primary"
      @click="pageSuivante()"
      :disabled="page === nbPagesTotal"
      >Suivant</md-button
    >
  </md-content>
  
</template>
<script>
export default {
  
}

</script>