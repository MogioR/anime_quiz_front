<template>
  <div class="container">
    <div class="container side_block" id="side_block">
      Side
    </div>
    <div class="container game_zone" id="gane_zone">
      <News_blok></News_blok>>
    </div>
  </div>
</template>


<script>
  // import { mapGetters, mapActions } from "vuex";
import News_blok from './components/game_zone/news_block.vue'
// import Authorisation from 'src_old/components/side_block/authorisation.vue';

  export default {
    name: 'App',
    components: {
      News_blok,
    }
  }
  </script>

<style>
.container {
    margin: 0px;
    padding: 0px;
    display: flex;
    overflow: overlay;
  
}
.side_block {
    width: 300px;
    min-width: 200px;
    height: 100vh;
    float: left;
    background: #383838;; 
}
.game_zone {
    width: 100vw;
    min-width: 600px;
    height: 100vh;
    flex: 1 0;
    background: #313131;
    overflow-y: overlay;
}
</style>
