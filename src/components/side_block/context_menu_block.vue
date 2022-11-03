<template>
    <div class="menu_container">
        <span class="text header" >{{header}}</span> 
        <div v-for="option of options" :key=option.id class="button menu_button" v-on:click="option.function">
            <span class="text">{{option.text}}</span>
        </div>
    </div>
  </template>
  
<script>
export default {
    name: 'ContextMenuBlock',
    data() {
        return {
            header: 'Меню',
            options: [
                {
                    text: 'Найти комнату',
                    function: function() {
                        alert('Test1');
                    }
                },
                {
                    text: 'Создать комнату',
                    function: function() {
                        alert('Test2');
                    }
                }
            ]
        }
    },
    methods: {
        func1: function() {
            alert('func1');
        },
        func2: function() {
            alert('func2');
        }
    }
}
</script>
  
<style scoped>
.menu_container {
    display: flex;
    flex-direction: column;
}
.text {
    width: 260px;
    text-align: center;
    font-family : 'Ubuntu';
    font-style: normal;
    margin: 10px;
}
  
.header {
    color: white;
    font-size: 25px;
    margin-bottom: 0px;
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
.button {
  font-size: 22px;
  background: #2B2B2B;
  width: 280px;
  
}

</style>