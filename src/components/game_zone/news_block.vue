<template>
    <div class="center_block">
        <div class="welcome_block">
            Welcome to the <br> MogioR Quiz
        </div>
        <div class="microblog_container">
            <div v-for="n of news" :key=n.id>
                <div>
                    {{n.title}}
                </div>
                <div>
                    {{n.body}}
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'NewsBlock',
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
    font-weight: 400;
    font-size: 128px;
    line-height: 147px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    text-align: center;
    height: 50%;
    width: 100%;
}
.microblog_container {
    background-color:blueviolet;
    margin-left: 80px;
    margin-right: 80px;
    justify-content: space-between;
    display: flex;
}
</style>