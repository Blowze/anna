<template>
  <div id="app">
    <!--  -->
    <vue-typer  v-if="button" @completed='onComplete' :text='["Анечка","Поздравляю", "Тебя","С новым годом!" ,"Наш драгоценный ", "Бриллиант", "Очень","Очень Очень Очень Очень Очень","Ну прям пипец как очень ....", "Много работает :(" , "Но ты больше остальных", "Заслужила заботы","и", "и и и и и и ", "Выпустить наружу Девочку", "Демонааааа","Поэтому я бы хотел занять","твои выходные и отправится","Вместе со мной и одной Селебрити","Ну мы поняли :)","В погоню за эмоциями","Ценим и любим","P.S Лешаааа"]' :repeat='0'   :pre-erase-delay='300'  :type-delay='100' erase-style='clear' caret-animation='expand'></vue-typer>
    <template v-else>
      <a href="https://yadi.sk/d/au6rdEQZ5ypTfg" target="_blank" class="btn">Получить подарок</a>
    </template>
  </div>
</template>

<script>
  export default {
    name: 'App',
    data() {
      return{
      button: true

      }
    },
  methods:{
   onComplete: function() {
     setTimeout(() => this.button = false, 1000)
    }
  }}
</script>

<style>
body{
  margin: 0;
  padding: 0;
}
#app{
  min-height: 100vh;
  background: #fff;
  padding: 0 20px;
  background: rgba(73,134,204,.08);
  display: flex;
  align-items: center;
  justify-content: center;
}
.text, .typed{
    margin: auto;
    font-family: -apple-system, BlinkMacSystemFont, Roboto, Open Sans, Helvetica Neue, 'Noto Sans Armenian', 'Noto Sans Bengali', 'Noto Sans Cherokee', 'Noto Sans Devanagari', 'Noto Sans Ethiopic', 'Noto Sans Georgian', 'Noto Sans Hebrew', 'Noto Sans Kannada', 'Noto Sans Khmer', 'Noto Sans Lao', 'Noto Sans Osmanya', 'Noto Sans Tamil', 'Noto Sans Telugu', 'Noto Sans Thai', sans-serif;
    font-size: 60px;
    font-weight: 600;
    line-height: 1.2;
}
.btn{
  display: inline-block;
    font-family: -apple-system, BlinkMacSystemFont, Roboto, Open Sans, Helvetica Neue, 'Noto Sans Armenian', 'Noto Sans Bengali', 'Noto Sans Cherokee', 'Noto Sans Devanagari', 'Noto Sans Ethiopic', 'Noto Sans Georgian', 'Noto Sans Hebrew', 'Noto Sans Kannada', 'Noto Sans Khmer', 'Noto Sans Lao', 'Noto Sans Osmanya', 'Noto Sans Tamil', 'Noto Sans Telugu', 'Noto Sans Thai', sans-serif;

    font-weight: 400;
    line-height: 1.5;
    color: #212529;
    text-align: center;
    text-decoration: none;
    vertical-align: middle;
    cursor: pointer;
    -webkit-user-select: none;
    -moz-user-select: none;
    user-select: none;
    background-color: transparent;
    border: 1px solid transparent;
    padding: .375rem .75rem;
    font-size: 1rem;
    border-radius: .25rem;
    transition: color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out;
        padding: .5rem 1rem;
    font-size: 1.25rem;
    border-radius: .3rem;
        font-weight: 600;
    color: #fff;
    background-color: #7952b3;
    border-color: #7952b3;
        padding: .8rem 2rem;
    font-weight: 600;
}
.btn:hover{
  color: #fff;
    background-color: #61428f;
    border-color: #61428f;

}
  
</style>