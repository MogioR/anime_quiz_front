<template>
    <div class="context_container">
        <div>
           Settings
        </div>
        <div>
            <AccountInfoBlock/>
        </div>
    </div>
</template>

<script>


import AccountInfoBlock from '@/components/side_block/account_info_block.vue'

export default {
  name: 'ContextBlock',
  components: {
    AccountInfoBlock
  },
  data() {
    return {}
  }
}
</script>

<style scoped>
.context_container {
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}
</style>