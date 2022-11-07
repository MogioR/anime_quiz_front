<template>
    <div class="container">
      <PlayerRoomItem v-for="n of players" :key=n.id>
      
      </PlayerRoomItem>
    </div>
</template>

<script>
import PlayerRoomItem from '@/components/game_zone/player_room_item.vue'

export default {
  name: 'LobbySearchBlock',
  components: {
    PlayerRoomItem
  },
  data() {
    return {
      players: [
        {},
        {},
        {},
        {},
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