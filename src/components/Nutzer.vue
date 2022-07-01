<template>
  <h3>Alle Verbindungen:</h3>
</template>
<script>
/*import axios in script tag of component where data is shown*/
  import axios from 'axios';
  export default 
  {
    name: 'Users',
    data() 
    {
      return 
      {
        users: null // should do the trick
      };
    },
    created: function() 
    {
      axios
        .get('https://jsonplaceholder.typicode.com/users')
        .then(res => {
          this.users = res.data;
        })
    }
  }
</script>
<style>
  h3 {
    margin-bottom: 5%;
  }
</style>