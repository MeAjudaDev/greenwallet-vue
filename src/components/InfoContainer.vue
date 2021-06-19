<template>
    <div class="container-name-email">
        <p id="name">Fulano de Tal</p>
        <p id="email" >meuemail@gmail.com</p>
    </div>
</template>

<script>

export default {
    name: 'InfoContainer'
}

</script>

<style scoped>
#name{
    font-size: 1rem;
    margin-bottom: 0.35rem;
}

#email{
    font-size:.75rem;
    color: #9B9FAA;
}
</style>