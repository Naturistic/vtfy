<template>

  <v-container fluid>
    <v-layout row wrap>

      <v-flex xs12 class="text-xs-center" mt-5>
      <div id="hero-section">
        <div class="search-bar">
          <div class="search-icon">
            <v-img src="../assets/search-1.svg" alt="" height="15px"></v-img>
          </div>
          <input type="text" placeholder="Search high-resolution photos">
        </div>
      </div>
      </v-flex>


    </v-layout>
  </v-container>
</template>
<script>
export default {
  // name: 'Landing'
};
</script>

<style>

* {
    padding: 0;
    margin: 0;
    font-family: 'Roboto', sans-serif;
}

#hero-section {
    background-image: url("../assets/desert_mountains.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    height: 400px;
    grid-column: 1/4;
    display: grid;
    grid-template-rows: 1fr 50px 1fr;
    grid-template-columns: 1fr 1fr 1fr;
}

.search-bar {
    grid-column-start: 2;
    grid-row-start: 2;
    display: flex;
    justify-content: center;
    align-items: center;
}

.search-bar input {
    background-color: white;
    height: 40px;
    width: 500px;
    outline: none;
    padding-left: 10px;
}

.search-icon{
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: white;
    height: 40px;
    padding: 0px 10px;
}

</style>
