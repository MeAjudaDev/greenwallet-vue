<template>
  <header>
    <div id="header">
      <div id="btn-avatar">
        <div id="btn"></div>
        <div id="avatar"></div>
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
}

h2 {
  width: 100%;
  text-align: center;
  font-size: 25px;
  color: #FFFFFF;   
}

</style>