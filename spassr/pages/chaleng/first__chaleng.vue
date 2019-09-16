<template>
    <div class="first__chaleng">
        <h1>@media</h1>
        <p>Для разработчиков у Google есть отличный инструмент для имитации мобильных устройств. Этот инструмент встроен в браузер Google Chrome. Для доступа к нему нужно нажать F12 в браузере (перейти в режим разработчика) и нажать на значок смартфона:</p>
        <img src="~static/chrome_smart.png" alt="">
        <p>Используя @media запросы сделать, читаемую страницу как на телефоне так и на ПК</p>
        <p>Пример:</p>
        <div class="block">
            <div><img src="~static/animatinAndJs.png" alt=""></div>
            <div><img src="~static/animatinAndJs.png" alt=""></div>
            <div><img src="~static/animatinAndJs.png" alt=""></div>
            <div><img src="~static/animatinAndJs.png" alt=""></div>
            <div><img src="~static/animatinAndJs.png" alt=""></div>
        </div>
    </div>
</template>


<style scope>
.first__chaleng{
    display: flex;
    flex-direction: column;
    padding: 100px;
}
img{
    width: 100%;
    max-width: 550px;
}
.block{
    display: flex;
    flex-direction: column;
}
.block div{
    padding: 10px
}
@media (min-width: 1024px ) {
    .block{
    display: flex;
    flex-direction: row;
    }
}
</style>