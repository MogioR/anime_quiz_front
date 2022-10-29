<template>
  <div class="container">
    <div class="container side_block" id="side_block">
      <AuthorisationBlock v-if="currentState == 'authorisation'"/>
      <ContextBlock v-if="currentState == 'lobby_search'"/>
    </div>
    <div class="container game_zone" id="gane_zone">
      <News_blok></News_blok>
    </div>
  </div>
</template>


<script>
  // import { mapGetters, mapActions } from "vuex";
import News_blok from './components/game_zone/news_block.vue'
import AuthorisationBlock from './components/side_block/authorisation_block.vue'
import ContextBlock from './components/side_block/context_block.vue';

  export default {
    name: 'App',
    components: {
      News_blok,
      AuthorisationBlock,
      ContextBlock
    },
    data() {
      return {
        currentState: 'lobby_search',
      }
    },
  }
  </script>

<style scoped>
.container {
    margin: 0px;
    padding: 0px;
    display: flex;
    overflow: overlay;
  
}
.side_block {
    width: 300px;
    min-width: 300px;
    height: 100vh;
    float: left;
    background: #383838;; 
}
.game_zone {
    width: 100vw;
    min-width: 600px;
    height: 100vh;
    flex: 1 0;
    background: #2B2B2B;
    overflow-y: overlay;
}
</style>
