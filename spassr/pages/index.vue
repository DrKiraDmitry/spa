<template>
  <div>
    <div class="DeusEx">
      <logo />  
      <div>
          <h1>Добро пожаловать в компанию MIKIRI</h1>
          <a href="#about">ПРОДОЛЖИТЬ</a>
      </div>             
    </div>
    <div id="about" class="AboutUs">
        <div class="logo">
            <p class="outside">У</p>
            <h2 class="logo__text">Наши услуги</h2>
        </div>
        <div  class="AboutUs__psiblock">
            <div class="block">
                <img src="~static/Vector.png" alt="">
                <div class="block__content">
                    <h1>Векторная Графика</h1>
                    <p>Занимаюсь созданием логотипов и иконок в векторной графике (в формате SVG), их можно использовать как на веб-страницах, так и для размещения на вещах
                    </p>
                    <button>Узнать больше</button>
                </div>
            </div>
            <div class="block">
                <img src="~static/animatinAndJs.png" alt="">
                <div class="block__content">
                    <h1>Анимация и Js</h1>
                    <p>
                        Красивая анимация, это не всегда легко, но она того стоит. Она сделает ваш сайт, живым и запоминающимся. Анимация это не только, выпадающие окна, можно заставить двигаться даже картины
                    </p>
                    <button>Узнать больше</button>
                </div>
            </div>
            <div class="block">
                <img src="~static/landing.png" alt="">
                <div class="block__content">
                    <h1>Верстка и Api</h1>
                    <p>
                        "Мне нужен сайт", но сайт это не только страница, ему еще нужна и логика, которая обрабатывается на сервере. Сайт может быть Одностраничный иначе, Лэндинг, а может сложным приложением в которым и чат, и управление заказами. Так что же нужно?
                    </p>    
                    <button>Узнать больше</button>
                </div>
            </div>
        </div>
    </div>
    <div class="Work">
            <h1>Почему выбирают нас</h1>
        <div class="Work__block">
            <div class="Work__psiblock">
                <i class="fas fa-laptop-code"></i>
                <h2>Ответсвенность и поддержка</h2>
            </div>
            <div class="Work__psiblock">
                <i class="fas fa-laptop-code"></i>
                <h2>Индивидуальный подход</h2>
            </div>
            <div class="Work__psiblock">
                <i class="fas fa-laptop-code"></i>
                <h2>Полная документация к проекту</h2>
            </div>
        </div>
    </div>
    <contact />
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import contact from '~/components/contact.vue'
export default {
  components: {
    Logo,
    contact
  }
}
</script>

<style>
/**/
.DeusEx{
    background: black;
    display: flex;
    flex-direction: column;
    justify-content: center;
    color: #f4ab42;
    text-align: center;
    padding: 80px 0;
    height: 80vh;
}
.DeusEx svg{
    width: 100%;
}
.DeusEx div{
    display: flex;
    flex-direction: column;
    margin: auto 0;
    padding: 10px;
    align-items: center;
}
.DeusEx a{
    border: 1px solid #f4ab42;
    background: transparent;
    color: #f4ab42;
    border-radius: 1rem;
    font-size: 15px;
    padding: 10px;
    text-decoration: none;
    width: fit-content;
}
@media(min-width: 768px){
    .DeusEx{
        flex-direction: row;
    }
    .DeusEx div{
        width: 100%;
    }
}
/**/
.AboutUs{
    display: flex;
    flex-direction: column;
    text-align: center;
    padding: 50px 0;
    background: #C8A2C8;
    color: #f4f4f4;
}
.AboutUs__psiblock{
    display: flex;
    flex-direction: column;
    align-content: space-between;
    width: 100%;
}
.AboutUs button{
    background: #520428;
    border: 2px solid #848bee;
    border-radius: 0.5rem;
    margin: auto;
    font-size: 20px;
    color: whitesmoke;
}
/*Карточки*/
.block{
    display: flex;
    flex-direction: column;
    margin: 10px 0;
    padding: 0 10px;
}
.block img{
    width: 100%;
    height: 100%; 
}
.block__content{
    position: relative;
    margin-top: -100px;
    background: linear-gradient(45deg, rgba(47, 42, 78, .8), rgba(80, 63, 118, .1));
    padding: 10px;
}
.block__content h1{
    font-size: 20px;
}
.block__content p{
    display: none;
}
/**/
@media(min-width: 768px){
    .block{
        margin: 0 15px;
        width: 100%;
        padding: 0;
    }
    .AboutUs__psiblock{
        flex-direction: row;
    }
}

/**/
.logo{
    align-items: center;
    display: flex;
    justify-content: center;
    text-align: center;
    padding: 10px;
}
.logo__text{
    position:absolute;
    margin: 0;
    font-size: 35px;
}
.outside{
    display: inline-block;
    position: relative;
    font-size: 200px;
    color: #ad8ead;
    margin: 0;
}
/**/

.Work{
    background: black;
    color: #F4AB41;
    display: flex;
    flex-direction: column;
    text-align: center;
}
.Work__block{
    display: flex;
    flex-direction: column;
}
.Work__psiblock{
    width: 100%;
    margin: 15px;
    border: 1px solid #F4AB41;
}

@media(min-width: 768px){
    .Work__block{
        flex-direction: row;
    }
}

</style>