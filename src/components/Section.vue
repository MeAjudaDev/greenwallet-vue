<template>
    <div>
    <section class="share">
        <h3 class="section-title">COMPARTILHAR CONTA</h3>
        <p class="section-phrase">Compartilhe o gerenciamento das despesas e receitas com a sua família</p>
        <ShareContainer/>    
    </section>
    </div>
</template>

<script>

import ShareContainer from './ShareContainer.vue'

export default {
    name: 'Section',
    components:{
        ShareContainer
        }
}
</script>

<style scoped>
    
</style>