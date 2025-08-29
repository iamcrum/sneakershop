<script>
import { computed } from 'vue'

export default {
  data(){
      return{
          
      }
  },
  
  methods:{
    checker(id){
      temp = new URL(`/${{id}}.webp`, import.meta.url).href
      return new URL(`/${{id}}.webp`, import.meta.url).href;
      console.log(temp)
    }
  }
  
  
};

</script>

<template>
  <div class = "but">

    <div class = "shopitem" id="1">
      <img src="/1.jpg"></img>
      <h3>Кеды NIKE Court Vision Mid Next Nature
      </h3>

      <p>для мужчин, повседневные спорт-стиль, высокие
      </p>
    </div>

    <div class = "shopitem" id="1">
      <img src="/2.jpg"></img>

      <h3>Кеды NIKE Court Vision Mid Next Nature
      </h3>

      <p>для мужчин, повседневные спорт-стиль, высокие
      </p>
    </div>

    <div class = "shopitem" id="1">
      <img src="/3.jpg"></img>

      <h3>Кеды NIKE Court Vision Mid Next Nature
      </h3>

      <p>для мужчин, повседневные спорт-стиль, высокие
      </p>
    </div>

    <div class = "shopitem" id="1">
      <img src="/4.jpg"></img>

      <h3>Кеды NIKE Court Vision Mid Next Nature
      </h3>

      <p>для мужчин, повседневные спорт-стиль, высокие
      </p>
    </div>

    <div class = "shopitem" id="1">
      <img src="/5.jpg"></img>

      <h3>Кеды NIKE Court Vision Mid Next Nature
      </h3>

      <p>для мужчин, повседневные спорт-стиль, высокие
      </p>
    </div>

    <div class = "shopitem" id="1">
      <img src="/6.jpg"></img>

      <h3>Кеды NIKE Court Vision Mid Next Nature
      </h3>

      <p>для мужчин, повседневные спорт-стиль, высокие
      </p>
    </div>

    <div class = "shopitem" id="1">
      <img src="/7.jpg"></img>
      <div class = "texted">

        <h3>Кеды NIKE Court Vision Mid Next Nature
        </h3>

        <p>для мужчин, повседневные спорт-стиль, высокие
        </p>
      </div>
    </div>

    <div class = "shopitem" id="1">
      <img src="/8.jpg"></img>

      <h3>Кеды NIKE Court Vision Mid Next Nature
      </h3>

      <p>для мужчин, повседневные спорт-стиль, высокие
      </p>
    </div>

  
    <button type="button" @click ="bebra(tempInt)">Отправить членикс</button>
  </div>

</template>

<style scoped>

div{  
  display: flex;
  margin-bottom: 10px;
  justify-content: center;
}

.but {
  grid-template-columns: repeat(4, 1fr);
  flex-wrap: wrap;
  padding-top: 10px;
  display: grid;
  justify-self: center;
  justify-content: center;
  align-items: center;
  color: aquamarine;
  border-color: black;
  border-style: dotted;
  
}

.but button{
  justify-self: center ;
  background-color:cornflowerblue;
  color: whitesmoke;
  height: 70px;
  width: 140px;
  font-family: 'Montserrat';
  font-weight: bold;
  font-size: large;
  border-radius: 7px;
  grid-column: 1 / -1;  
  padding: 15px; 
}


.shopitem{
  width: 170px;
  height: 300px;
  justify-content: center;
  align-items: center;
  background-color: rgb(255, 255, 255);
  flex-direction: column;
  text-align: center;
  margin: 10px;
  margin-left: 40px;
  margin-right: 40px;
  border-radius: 10px;
}

.shopitem img{
  
  width: 140px;
  border-style: solid;
  border-color: black;
  border-radius: 10px;
  -moz-transition: all 0.1s ease-out;
  -o-transition: all 0.1s ease-out;
  -webkit-transition: all 0.1s ease-out;
   transition: all 0.1s ease-out;
}

.shopitem img:hover{
  border-color: rgb(112, 226, 255);
  -webkit-transform: scale(1.05);
 -moz-transform: scale(1.05);
 -o-transform: scale(1.05);
 transform: scale(1.05);

}

.shopitem h3{
  font-family: "Montserrat";
  font-weight: bold;
  color: rgb(0, 0, 0);
  font-size: medium;
  align-content: le;
  padding: 15px;
  text-align: left;
}

.shopitem p{
  font-family: "Montserrat";
  font-weight: normal;
  color: rgb(0, 0, 0);
  font-size: medium;
  align-content: center;
  margin-bottom: 10px;
  text-align: right;
  margin-right: 15px;
}

.texted{
  flex-direction: column;
}

input{
  height: 24px;
  border-radius: 100px;
  text-align: center;
  font-family: 'Montserrat';
}

@font-face {
  font-family: 'Montserrat';
  src: url("fonts/Montserrat-Bold.ttf") format('truetype');
  font-weight: bold;
}

@font-face {
  font-family: 'Montserrat';
  src: url("fonts/Montserrat-Regular.ttf") format('truetype');
  font-weight: normal;
}

h1{
  margin-top: 100px;
  display: flex;
  justify-content: center;
  color: whitesmoke;
  font-weight: lighter;
  font-size: 500%;
  font-family: 'Montserrat';
  font-weight: normal;
}
</style>
