<template>
    <div class="room_player_item">
        lol
    </div>
</template>

<script>
export default {
  name: 'LobbySearchItem',
  data() {
    return {
    }
  },
  props: {
    'name': String, 
    'room_size': Number,
    'player_count': Number,
    'password': Boolean,
    'state': String
  }
}
</script>

<style scoped>
.room_player_item {
    width: 190px;
    height: 300px;
    border-radius: 9px;
    background: #696969;
    margin: 15px;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}
.room_avatar {
  width: 170px;
  height: 170px;
  margin: 10px;
  border-radius: 9px;
  background-color: #101010;
  display: flex;
  justify-content: flex-end
}
.header {
  margin-top: 5px;
}

.text {
    text-align: center;
    font-family : 'Ubuntu';
    font-style: normal;
    font-size: 20px;
    margin-bottom: 5px;
    color: white;
}
.num_players_text {
  margin: 10px;
}
.connect_room_button {
  background: #2B2B2B;
  width: 170px;
  margin: 0px 10px 0px 10px;
  border-radius: 5px;
}
</style>