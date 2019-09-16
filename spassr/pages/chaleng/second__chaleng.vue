<template>
    <div class="second__chaleng">
        <h1>Flex-Box</h1>
        <p>Научиться использовать display:flex</p>
        <p>С помощью флексов сделать страницу</p>
        <p>или хотяб так</p>
        <div class="primer">
            <img src="~static/animatinAndJs.png" alt="">
            <div>
                <img src="~static/animatinAndJs.png" alt="">
                <img src="~static/animatinAndJs.png" alt="">
            </div>
        </div>
    </div>
</template>

<style scope>
.second__chaleng{
    display: flex;
    flex-direction: column;
    padding: 100px;
}
img{
    width: 100%;
    object-fit: contain;
}
.primer{
    display: flex;
    width: 100%;
    background: black;
}
.primer div{
    display: flex;
    flex-direction: column;
    width: 100%;
    height: 100%;
}
</style>