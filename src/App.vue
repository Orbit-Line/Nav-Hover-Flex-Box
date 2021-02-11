<template>
  <div id="app">
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 

    <header>
      <nav>
       <ul> 
          <li><a href="#"><span class="primero"><i class="icon icon-house"><img src="https://img.icons8.com/android/24/000000/dog-house.png"/></i></span>Inicio</a></li>
          <li><a href="#"><span class="segundo"><i class="icon icon-tag"><img src="https://img.icons8.com/ios-glyphs/30/000000/sale-price-tag.png"/></i></span>Categorías</a>
            <ul>
               <li><a href="#">Item #1</a></li>
               <li><a href="#">Item #2</a></li>
            </ul>
          </li>
          <li><a href="#"><span class="tercero"><i class="icon icon-suitcase"><img src="https://img.icons8.com/metro/26/000000/suitcase.png"/></i></span>Servicios</a>
               <ul>
               <li><a href="#">Item #3</a></li>
               <li><a href="#">Item #4</a></li>
               <li><a href="#">Item #5</a></li>
               </ul>
              </li>
          <li><a href="#"><span class="cuarto"><i class="icon icon-text"><img src="https://img.icons8.com/material/24/000000/rich-text-converter.png"/></i></span>Acerca</a></li>
           
          <li><a href="#"><span class="quinto"><i class="icon icon-gmail"><img src="https://img.icons8.com/android/24/000000/gmail-login.png"/></i></span>Contacto</a></li>
       </ul>
      </nav>
    </header>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
  
  }
}
</script>

<style scoped>
#app {
  font-family: Arial, sans-serif
 -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
}
* {
  margin: 0;
  padding: 0;
}
header {
  width: 100%;
} 
nav {
  margin:auto;
  width: 90%;
  max-width: 1000px;
}
nav ul {
  list-style: none;
}
nav > ul {
  display: table;
  width: 100%;
  background: #9e9e9e;
  position: relative;
}

nav > ul li {
  display: table-cell;
}
   /*SubMenu*/
nav > ul > li:hover > ul {
   display: flex;
   flex-direction: column;
   align-items: stretch;
   height: 300%;
   width: 15%;
   }
nav > ul > li > ul   {
   display: flex;
   flex-direction: column;
   align-items: stretch;
   position: absolute;
   background: darkblue;
   left: 50;
   right:30;
   height:0%;

  -webkit-transition: all .3s ease;
  -moz-transition: all .3s ease;
  -ms-transition: all .3s ease;
  -o-transition: all .3s ease;
  transition: all .3s ease;
   
}

nav > ul li  a {
  color: #fff;
  display: block;
  line-height: 20px;
  padding: 20px;
  position: relative;
  text-align: center;
  text-decoration: none;
  -webkit-transition: all .3s ease;
  -moz-transition: all .3s ease;
  -ms-transition: all .3s ease;
  -o-transition: all .3s ease;
  transition: all .3s ease;
}
nav > ul > li > ul > li a:hover {
  display: flex;
  flex-direction: column;
  background: chartreuse;
}
nav > ul > li > a span {
  background: #174459;
  display: block;
  height: 100%;
  width: 100%;
  left: 0;
  position: absolute;
  top: -60px;
  -webkit-transition: all .3s ease;
  -moz-transition: all .3s ease;
  -ms-transition: all .3s ease;
  -o-transition: all .3s ease;
  transition: all .3s ease;
}
nav > ul > li > a span .icon {
   display: block;
   line-height: 60px;
}
nav > ul > li > a:hover > span {
  top:0;
}
   /*Colores*/

nav ul li a .primero{
  background: aqua;
}  
nav ul li a .segundo{
  background: rgb(86, 70, 233);
}
nav ul li a .tercero {
  background: cornflowerblue;
}
nav ul li a .cuarto{
  background:coral
}
nav ul li a .quinto{
  background: rgb(171, 221, 34);
}
  @media screen and (max-width: 700px){
header  {
  margin: auto;
} 
}
</style>


