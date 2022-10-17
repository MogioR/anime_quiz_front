<template>
  <div class="microblog_item_main">
    <div class="microblog_item_title">
        {{title}}
    </div>
    <div class="microblog_item_body">
      {{body}}
    </div>
  </div>
</template>

<script>
export default {
  name: 'MicroblogItem',
  props: {
    'title': String, 
    'body': String
  }
}
</script>

<style scoped>
.microblog_item_main {
  margin: 10px;
  width: 300px;
  height: 330px;
  background-color: #272727;
  border-radius: 14px;
  border: 4px solid #4b4b4b;

  display: flex;
  flex-direction: column;
}
.microblog_item_title {
  height: 70px;
  width: 100%;
  border-bottom: 4px solid #4b4b4b;
  display: flex;
}

.microblog_item_body {
  display: flex;
  height: 100%;
  width: 100%;
}
</style>