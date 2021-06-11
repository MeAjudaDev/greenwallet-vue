<template>
    <div class="name-and-status">
        <p class="member-name">Fulana da Silva Sauro</p>
        <p class="member-status">último acesso em 27/04/2021 às 14:19</p>
        <p class="member-type">Principal</p>
    </div>   
</template>

<script>

export default {
    name: 'FamilyMember'
}

</script>

<style scoped>

    .name-and-status{
        margin-left: .8rem;
    }

    .member-status{
        color: #9B9FAA;
        font-size: 0.7rem;
    }

    .member-type {
        font-size: 0.7rem;
        color: #01C9B8;
    }
</style>
