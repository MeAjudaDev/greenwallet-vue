<template>
    <button v-bind:class= "buttonStyle" type="type">{{tag}}</button>
</template>

<script>
export default {
    name: 'Button',
    props: ['mode', 'tag', 'type'],

    computed: {
    
        buttonStyle() {
            if(this.mode == 'save') {return 'btn-save';}
            else if(this.mode == 'return') {return 'btn-return';}
            else { return '';}
        }
    }
}


</script>

<style>

    .btn-save, .btn-return{
        margin: .2rem 0;
        width: 100%;
        padding: .6rem 0;  
    }

    .btn-return{
        background-color: #FFFFFF;
        color: #01C9B8;
        border: 1px solid #01C9B8;
    }

    .btn-save{
        border: 1px solid #01C9B8;
        background-color: #01C9B8;
        color: #FFF;
    }
    
</style>