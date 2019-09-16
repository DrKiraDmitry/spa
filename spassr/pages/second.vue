<template>
    <div class="template__second">
        <div class="TwoImg">
            <div class="ImgBlock">
                <div class="blok1">
                    <img src="~static/darkside/1.jpg" alt="">
                    <img :class="{opacity1: check1 === true}" id="Dside" src="~static/darkside/2.jpg" alt="">
                </div>
                <div class="text">
                    <p>
                        На войне было проще,<br> Я знал, кто враг, кто друг.
                    </p>
                </div>
                <div class="box">
                    <input type="checkbox" class="checkbox" id="checkbox" @click="check1 = !check1">
                    <label for="checkbox"></label>
                </div>
            </div>
            <div class="ImgBlock">
                <div class="blok1">
                    <img src="~static/darkside/41.jpg" alt="">
                    <img :class="{opacity1: check2 === true}" id="Dside2" src="~static/darkside/42.jpg" alt="">
                </div>
                <div class="text">
                    <p>
                    Относись к людям так,<br> Как хочешь чтоб относились к тебе.
                    </p>
                </div>
                <div class="box">
                    <input type="checkbox" class="checkbox" id="checkbox2" @click="check2 = !check2">
                    <label for="checkbox2"></label>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
            check1:true,
            check2:true,
        }
    }
}
</script>
<style>
.TwoImg{
    padding: 100px 0;
}
.template__second{
    background: url(~static/darkside/4978587317_71dff37ae1_b.jpg);
    display: flex;
}
.blok1 {
  display: flex;
  color: #FFF;
  cursor: pointer;
}
#Dside, #Dside2{
  position: relative;
  left: -100%;
  transition: 3s;
}
.opacity1{
    opacity: 0;
}
img{
  width: 100%;
  height: 100%;
}
.ImgBlock{
  display: flex;
  flex-direction: column;
  max-width: 500px;
  margin: auto;
}
.box{
  padding: 40px 0px;
  text-align: center;
}
.text{
  position: relative;
  margin-top: -61px; 
  z-index: 3;
  background: linear-gradient(45deg, rgba(47, 42, 78, .8), rgba(80, 63, 118, .1));
}
.text p{
  font-size: 12px;
  color: white;
  padding: 5px 10px;
}
/**/
.checkbox {
  position: absolute;
  z-index: -1;
  opacity: 0;
  margin: 10px 0 0 20px;
}
.checkbox + label {
  position: relative;
  padding: 0 0 0 60px;
  cursor: pointer;
}
.checkbox + label:before {
  content: '';
  position: absolute;
  top: -4px;
  left: 0;
  width: 50px;
  height: 26px;
  border-radius: 13px;
  background: #CDD1DA;
  box-shadow: inset 0 2px 3px rgba(0,0,0,.2);
  transition: .2s;
}
.checkbox + label:after {
  content: '';
  position: absolute;
  top: -2px;
  left: 2px;
  width: 22px;
  height: 22px;
  border-radius: 10px;
  background: #FFF;
  box-shadow: 0 2px 5px rgba(0,0,0,.3);
  transition: .2s;
}
.checkbox:checked + label:before {
  background: #9FD468;
}
.checkbox:checked + label:after {
  left: 26px;
}
.checkbox:focus + label:before {
  box-shadow: inset 0 2px 3px rgba(0,0,0,.2), 0 0 0 3px rgba(255,255,0,.7);
}
@media(min-width: 768px)
{
  .TwoImg{
    display: flex;
    flex-direction: row;
    margin: 0 auto;
  }
  .ImgBlock{
    margin: 0 20px;
  }
}    
</style>