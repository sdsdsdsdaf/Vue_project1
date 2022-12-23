<template>
  <img alt="Vue logo" src="./assets/logo.png">

  <div>
    <!--{{데이터}}-->
    <h4>XX 원룸</h4>
    <p>{{ price1 }} 만원</p>
  </div>
  <div>
    <h4>XX 원룸</h4>
    <p>{{ price2 }} 만원</p> 
  </div>
  
</template>

<script>



export default {
  name: 'App',
  //데이터 바인딩: JS데이터를 HTML에 (데이터 바인딩: object 자료를 html 안에)
  data(){
    return {
      //이 return 괄호 안에 js데이터 집어넣어야 함 (TO DO 그렇다면 함수 식으로 만들어 다른 함수 return 가능>?)
      price1: 60, //Object 자료형 인덱스: 값
      price2: 70
    }
  },
  components: {
    
  }
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
</style>
