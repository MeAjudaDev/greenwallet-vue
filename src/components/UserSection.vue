<template>    
    <section class="share">                    
        <h3 class="section-title">EDITAR USUÁRIO 
            <button id="btn-config" type="button">
            <img src="../assets/btn-config.svg" alt="">
            </button>
        </h3>
        <div class="container-user">
            <Avatar />
            <InfoContainer />
        </div>                  
    </section>    
</template>

<script>

import Avatar from './Avatar.vue';
import InfoContainer from './InfoContainer.vue';


export default {
    name: 'UserSection',
    components: {
        Avatar,
        InfoContainer,
    }
}
</script>

<style scoped>

.container-user{
  display: flex;
  justify-content: center;
  align-items: center;
}

</style>