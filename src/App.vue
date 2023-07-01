<template>
  <div id="app">
    <ul>
      <li v-for="item in items" >
        <p>{{item.title}}</p>
        <p>{{item.subinfo}}</p>
        <p><img :src=item.conimg /></p>
        <img src="./assets/logo.png">
      </li>
    </ul>
    <!-- <router-view/> -->
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      items:[
        {
          title:'셀프 도배시공과 싱크대 페인트리폼으로 변화 준 주방인테리어',
          subinfo:'시크한까미',
          conimg:'./assets/logo.png'
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
