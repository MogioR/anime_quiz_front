<template>
  <div class="microblog_item_main">
    <div class="microblog_item_title">
      <span v-html="title"></span>
    </div>
    <div class="microblog_item_body">
      <span v-html="body"></span>
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

  flex-wrap: wrap;
  flex-direction: column;
}
.microblog_item_title {
  height: 70px;
  width: 100%;
  border-bottom: 4px solid #4b4b4b;
  display: flex;
  justify-content: space-around;
  align-items: center;

  color: white;
  font-family : 'Ubuntu';
  font-style: normal;
  font-size: 30px;

}

.microblog_item_body {
  display: flex;
  height: 230px;
  width: 270px;

  display: flex;
  justify-content: space-around;
  align-items: center;

  color: rgb(138, 138, 138);
  font-family : 'Ubuntu';
  font-style: normal;
  font-size: 20px;
  text-align: center;
  padding: 15px;
}

</style>