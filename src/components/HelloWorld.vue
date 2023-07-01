<template>
  <div class="hello">
   test
  </div>
</template>

<script>
import { Axios } from 'axios';
export default {
  name: 'HelloWorld',
  data () {
    return {
     
    }
  },
  methods: {
    getData () {
      return Axios
        .get('./assets/data.json')
        .then(res => {
          console.log(res)
        })
        .catch(error => {
          console.error(error)
        })
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
