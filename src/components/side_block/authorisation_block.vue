<template>
    <div class="container">
        <div class="center">
            <LoginInputBlock></LoginInputBlock>
        </div>
        <div class="bottom">
            <LoginButtomBlock></LoginButtomBlock>
        </div>
    </div>
</template>

<script>
import LoginInputBlock from '@/components/side_block/login_input_block.vue';
import LoginButtomBlock from '@/components/side_block/login_button_block.vue';

export default {
  name: 'AuthorisationBlock',
  components: {
    LoginInputBlock,
    LoginButtomBlock
  },
  data() {
    return {}
  }
}
</script>

<style scoped>
.container {
    width: 100%;
    height: 100%;
    display: flex;
    
    flex-direction: column-reverse;
    justify-content: space-between;
    align-items: center;

}
.center {
    width: 300px;
    top: 40%;
    position: absolute;

    display: flex;
    align-items: center;
}

.bottom {
    width: 300px;

    display: flex;
    align-items: center;
}
</style>