<template>
  <div id="app">
    <div id="parentDiv">
      <div v-for="(item, index) in hero" :key="index" id="mobileLegend"> 
        <h2>Nama Hero : {{item.nama}}</h2>
        <h2>Role : {{item.role}}</h2>
        <h2 v-if="item.role == 'Mage'">Lane : Mid Lane</h2>
        <h2 v-else-if="item.role == 'Fighter'">Lane : Exp Lane</h2>
        <h2 v-else-if="item.role == 'Assasin'">Lane : Jungle</h2>
        <h2 v-else-if="item.role == 'Marksman'">Lane : Gold Lane</h2>
        <h2 v-else>Lane : Roam</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data : function(){
    return{
      hero : [
        {
          nama : "Luo Yi",
          role : "Mage",
        },
        {
          nama : "Yu Zhong",
          role : "Fighter"
        },
        {
          nama: "Ling",
          role : "Assasin"
        },
        {
          nama: "Beatrix",
          role: "Marksman"
        },
        {
          nama: "Rafaela",
          role: "Support"
        }
      ]
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

#parentDiv {
  display: flex;
  align-items: center;
  flex-direction: column;
}

#mobileLegend{
  border: solid 1px black;
  width: 30%;
  display: flex;
  flex-direction: column;
  align-items: start;
  padding-left: 10px;
  padding-top: 10px
}
</style>