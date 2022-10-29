<template>
    <div class="container">
        <span class="text button">Создать новую учетную запись</span>
        <span class="text button">Восстановить учетную запись</span>
    </div>
</template>

<script>
export default {
  name: 'LoginButtomBlock',
  data() {
    return {}
  }
}
</script>

<style scoped>

.container {

}
.text {
  text-align: center;
  font-family : 'Ubuntu';
  font-style: normal;
  margin: 5px;
  margin-bottom: 20px;
}


.button {
  font-size: 18px;
  color: rgb(200, 200, 200);
}
</style>