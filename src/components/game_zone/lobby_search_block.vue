<template>
    <div class="container">
        <LobbySearchItem/>
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
    }
  }
}
</script>

<style scoped>
.container {
    width: 100%;
    height: 100%;

    display: flex;
}
</style>