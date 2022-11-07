<template>
    <div class="account_container">
        <span class="text header">Аккаунт</span>
        <div class="button menu_button"> 
            <span class="text">Друзья</span>
        </div>
        <div class="button menu_button">  
            <span class="text">Настройки</span>
        </div>
        <div class="avatar_backplate">
            <div class="avatar">
                
            </div>
            <div class="stats">
                <div>
                    <span class="text account_nickname">Mogior</span>
                    <div class="account_info"><span class="text">Уровень </span> <span class="text"> 10 </span></div>
                    <div class="account_info"><span class="text">Опыт </span> <span class="text">12</span></div>
                    <div class="account_info"><span class="text">Статус</span><span class="text">Онлайн</span></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>


export default {
  name: 'AccountInfoBlock',
  components: {

  },
  data() {
    return {}
  }
}
</script>

<style scoped>
.account_container {
    width: 280px;
    height: 270px;
    margin: 10px 10px 0px 10px;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.header {
  color: white;
  font-size: 25px;
}

.button {
  font-size: 22px;
  background: #2B2B2B;
  width: 280px;
  
}

.menu_button {
    width: 280px;
    height: 40px;
    margin: 10px 10px 0px 10px;
    border-radius: 9px;
    font-size: 20px;
    color: rgb(204, 204, 204);

    display: flex;
    justify-content: space-around;
    align-items: center;
}

.avatar_backplate {
    width: 280px;
    margin: 10px;
    height: 120px;
    border-radius: 9px;
    background: #2B2B2B;
    display: flex;
}
.avatar {
    height: 110px;
    width: 110px;
    margin: 5px;
    border-radius: 9px;
    background-color: #101010;
}
.stats {
    width: 160px;
}
.text {
  text-align: center;
  font-family : 'Ubuntu';
  font-style: normal;
  color: white;
  display: block;
}

.account_nickname {
    margin-top: 10px;
    font-size: 25px;
}
.account_info {
    display: flex;
    text-align: left;
    justify-content: space-between;
    margin: 5px 10px 0px 5px;
}
</style>