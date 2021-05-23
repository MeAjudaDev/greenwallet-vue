<template>
  <header>
    <div id="header">
      <div id="btn-avatar">
          <img src="./assets/menu-mobile.svg" id="menu-mobile"/>
          <img class="avatar" src="./assets/teste.png" alt="avatar">          
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
    <div class="container-user">
      <div class="container-img">
        <img class="avatar avatar-config" src="./assets/teste.png">
      
      </div>
      <div class="container-name-email">
        <p id="name">Fulano de Tal</p>
        <p id="email" >meuemail@gmail.com</p>
      </div>
    </div>
    <section class="share">
      <h3 class="section-title">COMPARTILHAR CONTA</h3>
      <p class="section-phrase">Compartilhe o gerenciamento das despesas e receitas com a sua família</p>
      <div class="share-container">
        <label for="input-share-account">E-mail</label>
        <input id="input-share-account" type="email">
        <button id="share-account" >+</button>
      </div>      
    </section>
    <section class="share">
      <h3 class="section-title">FAMÍLIA 
        <button id="btn-config" type="button">
          <img src="./assets/btn-config.svg" alt="">
        </button>               
      </h3>
      <div class="family-member">        
        <img class="avatar member-avatar" src="./assets/teste.png" alt="avatar">
        <div class="name-and-status">
          <p class="member-name">Fulana da Silva Sauro</p>
          <p class="member-status">último acesso em 27/04/2021 às 14:19</p>
          <p class="member-type">Principal</p>
        </div>        
      </div>
      <div class="family-member">        
        <img class="avatar member-avatar" src="./assets/teste.png" alt="avatar">
        <div class="name-and-status">
          <p class="member-name">Fulana da Silva Sauro</p>
          <p class="member-status">último acesso em 27/04/2021 às 14:19</p>
          <p class="member-type">Principal</p>
        </div>        
      </div>
    </section>  
  </main>
  <footer>
    <button class="btn-save" type="button">Salvar</button>
    <button class="btn-return" type="button">Voltar</button>
  </footer>
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

.avatar {
  width: 2.2rem; 
  height: 2.2rem;
  border-radius: 50%;
  border: none;  
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

.container-user{
  display: flex;
  justify-content: center;
  align-items: center;
}
.avatar-config{
  width: 5rem;
  height: 5rem;
  margin-right: .8rem;
}
#name{
  font-size: 1rem;
  margin-bottom: 0.35rem;

}
#email{
  font-size:.75rem;
  color: #9B9FAA;
}

.share{
  padding: 1rem;
}

.section-title {
  display: flex;
  align-items: center;
  justify-content: space-between;
  color: #9B9FAA;
  border-bottom: solid 2px #9B9FAA;
  padding-bottom: .4rem;
  margin-bottom: .75rem;
}

.section-phrase{
  padding-bottom: .75rem;
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

#btn-config {  
  background: none;
  border: none;
}

.family-member{
  display: flex;
  line-height: 1.1rem;
  margin-bottom: .8rem;   
}

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

footer{
  padding: 1rem;
}

.btn-save, .btn-return{
  margin: .2rem 0;
  width: 100%;
  padding: .6rem 0;  
}

.btn-save{
  border: 1px solid #01C9B8;
  background-color: #01C9B8;
  color: #FFF;
}

.btn-return{
  background-color: #FFFFFF;
  color: #01C9B8;
  border: 1px solid #01C9B8;
}



</style>