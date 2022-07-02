<template>

  <div class="container">
     <div class="columns medium-4">
      <div class="card">
        "Q:Alle Karten liegen auf Tisch"   
      </div>
      </div>
      <h3>Alle Spielkarten:</h3>
      <!-- SYMBOLS https://www.w3schools.com/charsets/ref_utf_symbols.asp -->
      <ul id="list">
        <li v-for="user in users" :key="user.id">
         {{user.name}} &#x29B6; &nbsp; &nbsp; &nbsp;<button class="primary" id="polar" >
          Karte zeigen &#x29A4;</button>
        </li>
      </ul>
  </div>
</template>
<script>
/*import axios in script tag of component where data is shown*/
  import axios from 'axios';
  import usersData from './nutzer.json';
  export default 
  {
     data() {
    return {
      users: usersData,
    };
  },
  }
   

</script>
<style>
ul{
   list-style-type: none;

}
 #list
  {
    color:red;
    font-weight: bold;
  }
  h3 {
    margin-bottom: 5%;
  }
  #polar:hover{
    background-color: black;
    color:lightgrey;
  }
   #polar{
    background-color: lightgrey;
    color:black;
  }
</style>