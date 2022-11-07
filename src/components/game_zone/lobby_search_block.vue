<template>
    <div class="container">
        <LobbySearchItem v-for="n of lobbyes" :key=n.id
        v-bind:name="n.name"
        v-bind:room_size="n.room_size"
        v-bind:player_count="n.player_count"
        v-bind:password="n.password"
        v-bind:state="n.state">
      </LobbySearchItem>
    </div>
</template>

<script>
import LobbySearchItem from '@/components/game_zone/lobby_search_item.vue'

export default {
  name: 'LobbySearchBlock',
  components: {
    LobbySearchItem
  },
  data() {
    return {
      lobbyes: [
        {
          "name": 'Комната 1',
          "room_size": 10,
          "player_count": 9,
          "password": false,
          "state": "В комнате" 
        },
        {
          "name": 'Blackfan and Loli',
          "room_size": 1,
          "player_count": 1,
          "password": false,
          "state": "В игре" 
        },
        {
          "name": 'Blackfan and Loli',
          "room_size": 1,
          "player_count": 1,
          "password": false,
          "state": "В игре" 
        },
        {
          "name": 'Blackfan and Loli',
          "room_size": 1,
          "player_count": 1,
          "password": false,
          "state": "В игре" 
        }
      ]
    }
  }
}
</script>

<style scoped>
.container {
    width: 100%;
    height: 100%;

    display: flex;
    justify-content: center;
    align-content: flex-start;
    flex-wrap: wrap;
}
.lol {
  background-color: blue;
}
</style>