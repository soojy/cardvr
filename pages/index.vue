
<template>
  <v-main class="welcome">
   <div class="container">
      <div class="welcome-wrapper">
            <div class="welcome-content animate__animated animate__backInLeft">
              <h1 class="welcome-title ">
                Виртуальные <br />
                Открытки
              </h1>
              <p class="welcome-text">
                Здесь вы найдёте уникальные виртуальные открытки<br />
                для друзей и знакомых<br />
                Создавайте собственные вирутальные открытки<br />
                Делитесь ими <br />
              </p>
              <button class="btn welcome-btn">Генерировать</button>
            </div>
            <div class="welcome-Aframe animate__animated animate__backInRight"></div>   
        </div>
   </div>
  </v-main>
</template>


<style lang="scss" >
@media (min-width: 1904px){
  .container {
      max-width: none;
  }
}
@media (min-width: 1264px){
  .container {
      max-width: none;
  }
}
@media (max-width: 1342px){
  .container {
      max-width: none;
  }
  .welcome {
    &-content{
      max-width: 50%;
    }
    &-Aframe{
      width: 400px !important;
    }
    &-title{
      font-size: 60px !important;
    }
    &-text{
      font-size: 20px !important;
    }
  }

}
@media (max-width: 873px){
  // .v-main__wrap{
  //   height: 200vh;
  // }
}
.welcome {
  .v-main__wrap{
    display: flex;
    align-items: center;
  }
  background: url("./assets/image/welcome-back.png") no-repeat;
  background-size: cover;
  height: 100vh;
  &-wrapper {
    color: white;
    width: 100%;
    justify-content: space-around;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
  }
  
  &-content{
    border-radius: 25px !important;
    min-height: 458px !important;
    padding: 20px 40px 20px 40px;
  }

  &-btn {
    padding: 27px 65px;
    font-size: 1.5em;
    line-height: 28px;
    transition: all ease-in-out .2s;
    &:hover{
        transform: translateY(-10%);
    }
  }
  &-title {
    font-size: 72px;
    line-height: 84px;
    font-weight: bold;
    margin-bottom: 63px;
    color: #fbfbfb;
  }
  &-text {
    // font-weight: 500;
    margin-bottom: 87px;
    font-size: 24px;
    line-height: 28px;
  }
  &-Aframe{
    width: 624px;
    min-width: 400px;
    min-height: 458px;
    height: 715px;
    background-color: white;
    border-radius: 50px;
  }
}
</style>

<script>
import 'animate.css';

export default {
  layout: "empty",
  mounted() {
    
  },
  data() {
    return {};
  },
};


</script>
