<template>

  <div class="menu">
    <!--for = "(값, 인덱스) vue 반복문 특징"-->
    <a v-for="(value, index) in menus" v-bind:key="index">{{ value }}</a> 
  </div>

  <div v-for = "(value, index) in products" v-bind:key="index">
    <!--{{데이터}}-->
    <!--: "안에 있는 데이터"-->
    <h4 :style="스타일">{{ value }}</h4>
    <p>{{prices[index]}} 만원</p>
  </div>
  
</template>

<script>



export default {
  name: 'App',
  //데이터 바인딩: JS데이터를 HTML에 (데이터 바인딩: object 자료를 html 안에)
  data(){
    return {
      //이 return 괄호 안에 js데이터 집어넣어야 함 (TO DO 그렇다면 함수 식으로 만들어 다른 함수 return 가능>?)
      prices: [50, 80, 70], //Object 자료형 인덱스: 값
      스타일: 'color: blue',
      products: ['역삼동 원룸', '천호동원룸', '마포구 원룸'],
      menus: ['Home', 'Shop', 'About']
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
  margin-top: 20px;
}

.menu{
  background: darkslateblue;
  padding: 15px;
  border-radius: 5px;
}
.menu a{
  color: white;
  padding: 10px;
}
</style>
