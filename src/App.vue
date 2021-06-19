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
    <UserSection />
    <ShareSection/>
    <FamilySection />  
    <Footer />
  </main>
</template>

<script>
  import Menu from './components/Menu.vue';
  import Avatar from './components/Avatar.vue';
  import NavOptions from './components/NavOptions.vue';
  import UserSection from './components/UserSection.vue';
  import ShareSection from './components/ShareSection.vue';
  import FamilySection from './components/FamilySection.vue';
  import Footer from './components/Footer.vue';  

export default {
  name: 'App',
  components: {
      Menu,
      Avatar,
      NavOptions,
      UserSection,
      ShareSection,
      FamilySection,
      Footer,      
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

.avatar-config{
  width: 5rem;
  height: 5rem;
  margin-right: .8rem;
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
  margin-bottom: 1.5rem;
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

</style>