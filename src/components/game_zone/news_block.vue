<template>
  <div class="center_block">
    <div class="welcome_block">
        Welcome to the <br> MogioR Quiz
    </div>
    <div class="microblog_container">
      <MicroblogItem 
        v-for="n of news" :key=n.id
        v-bind:title="n.title"
        v-bind:body="n.body">
      </MicroblogItem>
    </div>
  </div>
</template>

<script>
import MicroblogItem from '@/components/game_zone/microblog_item.vue'

export default {
  name: 'NewsBlock',
  components: {
    MicroblogItem
  },
  data() {
    return {
      news: [
        {
            'title': 'Title1',
            'body': 'Body1'
        },
        {
            'title': 'Title2',
            'body': 'Body2'
        },
        {
            'title': 'Title3',
            'body': 'Body3'
        },
        {
            'title': 'Title4',
            'body': 'Body2'
        },
        {
            'title': 'Title3',
            'body': 'Body3'
        },
        {
            'title': 'Title2',
            'body': 'Body2'
        },
        {
            'title': 'Title3',
            'body': 'Body3'
        },
        {
            'title': 'Title2',
            'body': 'Body2'
        },
        {
            'title': 'Title3',
            'body': 'Body3'
        },
        {
            'title': 'Title2',
            'body': 'Body2'
        },
        {
            'title': 'Title3',
            'body': 'Body3'
        },
        {
            'title': 'Title2',
            'body': 'Body2'
        },
        {
            'title': 'Title3',
            'body': 'Body3'
        }
      ]
    }
  }
}
</script>

<style scoped>
.center_block {
    width: 100%;
}
.welcome_block {
    color: white;
    font-family : 'Ubuntu';
    font-style: normal;
    font-size: 7vw;
    display: flex;
    justify-content: space-around;
    align-items: center;
    text-align: center;
    height: 50%;
    width: 100%;
}
.microblog_container {
    /* background-color:blueviolet; */
    margin-left: 80px;
    margin-right: 80px;
    
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    align-items: flex-end;
    justify-content: center;
}
</style>