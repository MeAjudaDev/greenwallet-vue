<template>
    <footer>
        <SaveButton />
        <BackButton />
    </footer>
</template>

<script>

import SaveButton from './SaveButton.vue'
import BackButton from './BackButton.vue'

export default {
    name: 'Footer',
    components:{
        SaveButton,
        BackButton
    }
}
</script>

<style>
    
.btn-save, .btn-return{
  margin: .2rem 0;
  width: 100%;
  padding: .6rem 0;  
}

</style>