<template>
    <section class="share">
        <h3 class="section-title">FAMÍLIA 
            <button id="btn-config" type="button">
            <img src="../assets/btn-config.svg" alt="">
            </button>               
        </h3>
        <div class="family-member">        
            <Avatar />
            <FamilyMember /> 
        </div>
        <div class="family-member">        
            <Avatar />
            <FamilyMember /> 
        </div>
    </section>  
</template>

<script>

import Avatar from './Avatar.vue';
import FamilyMember from './FamilyMember.vue';

export default {
    name: 'FamilySection',
    components: {
        Avatar,
        FamilyMember,
    }
}

</script>

<style scoped>


</style>
