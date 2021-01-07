<template>
  <div class="hello">
    <div class="icons">
      <img src="../assets/logo.png" />
    </div>
    <h1 class="headerText">Test</h1>
    <div class="cardt">
      <h2 class="title">О нас</h2>
      <p class ="text">
        Lorem Ipsum - это текст-"рыба", часто используемый в печати и
        вэб-дизайне. Lorem Ipsum является стандартной "рыбой" для текстов на
        латинице с начала XVI века. В то время некий безымянный печатник создал
        большую коллекцию размеров и форм шрифтов, используя Lorem Ipsum для
        распечатки образцов. Lorem Ipsum не только успешно пережил без заметных
        изменений пять веков, но и перешагнул в электронный дизайн. Его
        популяризации в новое время послужили публикация листов Letraset с
        образцами Lorem Ipsum в 60-х годах и, в более недавнее время, программы
        электронной вёрстки типа Aldus PageMaker, в шаблонах которых
        используется Lorem Ipsum
      </p>
    </div>
    
  <div class="box"></div>
    <div class="box"></div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  display: flex;
  flex-direction: column;
  background-color: rgba(200, 238, 238, 0.993);
  max-width: 100%;
  height: 300px;
}

img {
  padding: 5px;
  max-height: 50px;
  max-width: 50px;
}

.headerText {
  font-family: "Staatliches", cursive;
  padding: 5px;
  text-align: center;
  color: orangered;
  font-size: 40px;
}

.cardt{
  display: flex;
  flex-direction: column;
  padding: 10px;
  border-radius: 3%;
  background-color: white;
  -webkit-box-shadow: 0px 10px 26px 0px rgba(0,0,0,0.75);
  -moz-box-shadow: 0px 10px 26px 0px rgba(0,0,0,0.75);
  box-shadow: 0px 10px 26px 0px rgba(0,0,0,0.75);
  margin-top: 25px;
}

.title{
  color: orangered;
  font-family: "Staatliches", cursive;
  font-size: 30px;  
}

.text{
  margin-top: -10px;
  font-family: 'Comfortaa', cursive;
  font-size: 15px;
}

.box{
  padding: 10px;
  width:100px ;
  min-height: 100px;
  margin: 1rem;
  animation: test  10s infinite;
}

@keyframes test {
 0% {
    background-image: url('../assets/img1.jpg');
    background-repeat: no-repeat;
       width: 100px;
          height: 100px;

  }
  100% {
        background-image: url('../assets/img2.jpg');
         background-repeat: no-repeat;
         width: 100px;
          height: 100px;
  }
}
</style>
