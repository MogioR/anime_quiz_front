<template>
    <div class="container">
        <span class="text button">Войти</span>
        <input type="password" id="pass_input" maxlength="32" class="text_input" placeholder="Пароль">
        <input type="text" id="login_input" maxlength="16" class="text_input" placeholder="Логин">
        <span class="text header">Авторизация</span>
    </div>
</template>

<script>
export default {
  name: 'LoginInputBlock',
  data() {
    return {}
  }
}
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
}

.text_input {
  width: 260px;
  height: 30px;
  border-radius: 7px;
  margin: 0 10px 5px 15px;

  color: #313131;
  font-size: 20px;
  text-align: center;
}

.text {
  width: 260px;
  /* margin: 0 10px 5px 15px; */

  text-align: center;
  font-family : 'Ubuntu';
  font-style: normal;
  margin: 10px;
}

.header {
  color: white;
  font-size: 25px;
}

.button {
  font-size: 22px;
  color: rgb(200, 200, 200);
}
</style>