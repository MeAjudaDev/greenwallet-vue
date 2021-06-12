<template>
  <header>
    <div id="header">
      <div id="btn-avatar">
        <Menu />
        <Avatar />
      </div>
      <h2>Configurações</h2>
    </div>
  </header>
  <main>
    <NavOptions />
    <div class="container-user">
      <div class="container-img">
        <Avatar />  
      </div>
      <div class="container-name-email">
        <p id="name">Fulano de Tal</p>
        <p id="email" >meuemail@gmail.com</p>
      </div>
    </div>
    <Section/>
    <FamilySection />  
  </main>
  <footer>
    <button class="btn-save" type="button">Salvar</button>
    <button class="btn-return" type="button">Voltar</button>
  </footer>
</template>

<script>
  import Menu from './components/Menu.vue';
  import Avatar from './components/Avatar.vue';
  import NavOptions from './components/NavOptions.vue';
  import Section from './components/Section.vue';
  import FamilySection from './components/FamilySection.vue';

export default {
  name: 'App',
  components: {
      Menu,
      Avatar,
      NavOptions,
      Section,
      FamilySection,
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
  /* width: 100%; */
  height: 2rem;    
  justify-content: space-between;
  align-items: center;
}

h2 {
  width: 100%;
  text-align: center;
  font-size: 25px;
  color: #FFFFFF;   
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