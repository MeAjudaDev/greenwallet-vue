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

</style>