<template>
    <div>
        <nav id="menu-options">
      <ul id="menu-options-list">
        <li class="menu-options-list-item active">Usuário</li>
        <li class="menu-options-list-item">Receitas</li>
        <li class="menu-options-list-item">Despesas</li>
      </ul>
    </nav>
    </div>
</template>

<script>
export default {
    name: "NavOptions"
}
</script>
<style scoped>

#menu-options-list{
  display: flex;
  justify-content: center;
  list-style-type:none;
}

.menu-options-list-item{
  font-size: 1.1rem;
  margin:0;
  padding: 1.5rem;
}

.active{
  color:#01C9B8;
  font-weight: bold;
}
</style>