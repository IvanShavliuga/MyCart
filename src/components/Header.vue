<template>
<header class="header">	
  <nav class="header__topline">
    <router-link to="/" class="header__logo">MyCart</router-link>
    <router-link to="/Cart" class="header__products"><span class="glyphicon glyphicon-shopping-cart"></span></router-link>
    <router-link to="/Products" class="header__products" id="all">ALL Products</router-link>
  </nav>
</header>
</template>
<style lang="scss">
@import '../assets/styles/vars.scss';
.header {
  background-image: url('../assets/images/header.jpg');
  height: 100vh;
  background-size: 100% 80%;
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
  &__products{
      margin-top: 1.3em;
       float: right;
       margin-left: 20px;
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

  }
</style>