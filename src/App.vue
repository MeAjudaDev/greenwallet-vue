<template>
  <header>
    <div id="header">
      <div id="btn-avatar">
          <img src="./assets/menu-mobile.svg" id="menu-mobile"/>
          <button id="avatar"></button>
      </div>
      <h2>Configurações</h2>
    </div>
  </header>
  <main>
    <nav id="menu-options">
      <ul id="menu-options-list">
        <li class="menu-options-list-item active">Usuário</li>
        <li class="menu-options-list-item">Receitas</li>
        <li class="menu-options-list-item">Despesas</li>
      </ul>
    </nav>
    <section id="share">
      <h3 class="section-title">COMPARTILHAR CONTA</h3>
      <p class="section-phrase">Compartilhe o gerenciamento das despesas e receitas com a sua família</p>
      <div class="share-container">
        <label for="input-share-account">E-mail</label>
        <input id="input-share-account" type="email">
        <button id="share-account" >+</button>
      </div>
      
    </section>
    
  </main>
</template>

<script>
export default {
  name: 'App',
  components: {

  }
}
</script>

<style>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Roboto;
  font-weight: normal;
}

body {
  width: 100vw;  
}

#header {
  background-color: #01C9B8;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  width: 100%;
  height: 9rem;
  padding: 25px 20px;
}

#btn-avatar {  
  display: flex;  
  width: 100%;
  height: 2rem;    
  justify-content: space-between;
  align-items: center;
}

#menu-mobile {
  width: 1.8rem;
}

#avatar {
  width: 2.2rem; 
  height: 2.2rem;
  border-radius: 50%;
  border: none;
  background: url('./assets/teste.png');
  background-size: cover;
}

h2 {
  width: 100%;
  text-align: center;
  font-size: 25px;
  color: #FFFFFF;   
}

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

#share{
  padding: 1rem;
}

.section-title {
  color: #9B9FAA;
  border-bottom: solid 2px #9B9FAA;
  padding-bottom: .4rem;
}

.section-phrase{
  padding: .75rem 0;
}

.share-container{
  align-items:center;
  display: flex;
  flex-wrap: wrap;
}

label{
  font-weight:bold;
  font-size: 1rem;
  margin-bottom: .3rem;
  width: 100%;
}

#input-share-account{
  background-color: #EBEBEB;
  border: none;
  padding: 1.2rem 1rem;
  width:min(80%,20rem);
}

#share-account{
  background-color:#01C9B8;
  border: none;
  border-radius:.1rem;
  color:#FFFFFF;
  font-weight: bold;
  font-size: 1.25rem;
  margin-left: .3rem;
  padding: .95rem 1.45rem;
}

</style>