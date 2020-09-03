<template>
<header class="header">	
  <nav class="header__topline">
    <router-link to="/" class="header__logo">MyCart</router-link>
    <router-link to="/Cart" class="header__products"><span class="glyphicon glyphicon-shopping-cart"></span></router-link>
    <router-link to="/Products" class="header__products" id="all">ALL Products</router-link>
  </nav>
  <div class="header__box">
    <h1 class="header__box-title">Welcome To MyCart</h1>		
	 <h2 class="header__box-subtitle">Your Shopping Cart</h2>
	 <router-link to="/Products" class="header__box-button"><span class="glyphicon glyphicon-tags" style="margin-right: 5px;"></span> Start Shopping</router-link>
  </div>
</header>
</template>
<style lang="scss">
@import '../assets/styles/vars.scss';
.header {
  background-image: url('../assets/images/header.jpg');
  height: 100vh;
  width: 100%;
  margin: 0 auto;
  background-size: cover;
  background-color: $bodybackground;
  background-position: center bottom;
  background-repeat: no-repeat;
  &__logo {
      margin-left: 1.2em;
      margin-top: 0.3em;
      float: left;
      font-size: 40px;
     font-family: Confetti;
     font-style: bolder;
      outline: none;
      color: $headertoplinecolor;
      text-decoration: none;
      margin-bottom: 0px;
      &:hover {     
      outline: none;
      color: #DB0960;
      text-decoration: none;
     }
     &:focus {
      outline: none;
      color: #DB0960;
      text-decoration: none;
     }
  }
  &__topline {
     background-color: rgba(0,28,32,0.8); 
     border-bottom: 2px solid red; 
     height: 100px;
  }
  &__products{
      margin-top: 1.3em;
       float: right;
       margin-right: 1.5em;
       outline: none;
       font-size: 18px;
      color: $headertoplinecolor;
      font-family: 'Comfortaa-Light';
      text-decoration: none;
     &:hover {
      outline: none;
      color: #DB0960;
      text-decoration: none;
     }
    &:focus {
      outline: none;
      color: #DB0960;
      text-decoration: none;
     }
     &:actived {
      outline: none;
      color: #DB0960;
      text-decoration: none;
     }
  }
    #all {
      border:1px solid ;
      border-color: $headertoplinecolor;
      border-radius: 5px;
      padding: 5px;
      font-size: 14px;
     }
     #all:hover {
      background-color: #DB0960;
      border-color: #DB0960;
       outline: none;
      color:white;
      text-decoration: none;
     }
     #all:focus {
      background-color: #DB0960;
      border-color: #DB0960;
       outline: none;
      color:white;
      text-decoration: none;
     }
    &__box {
      width: 70vw;
      height: 60vh;
      margin: 150px auto 50px auto;
      text-align: center;
      &-title {
        font-size: 80px;
        font-weight: bold;
        color: $colortitle;
        text-shadow: 5px 0px 15px #df67c0;
      } 
      &-subtitle {
        font-size: 40px;
        font-style: italic;
        color: $colortitle;
        margin-bottom: 100px;
      }
      &-button {
        background-color: transparent;
        border:1px solid #df67c0;
        font-size: 22px;
        font-weight: bold;
        color: #df67c0;
        text-decoration: none;
        padding: 10px;
        border-radius: 5px;
        margin-top: 60px;
        &:hover {
          background-color: #df67c0;
          color: white;
          text-decoration: none;
        }   
      }
   
    }
  }
</style>