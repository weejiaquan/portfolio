<template>
  <div id="app">
    <div id="nav">
      <li> <router-link to="/">Home</router-link> </li>
      <li> <router-link to="/about">About</router-link> </li>
    </div>
     <transition appear name="fade" mode="out-in">
    <router-view />
    </transition>
  </div>

</template>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-left: 13%; 
}

#nav {
  background-color: aquamarine;
  position: fixed;
  height: 100%;
  left: 0;
  top: 0;
  width:12%;
  z-index:1;
}

li {
  list-style-type: none;
  margin: 2em;
  font-size: 1.5vw;
  text-align: center;
}

li:hover{
  transform: scale(1.5);
  transition: transform 0.3s;
}

li:not(:hover){
  transform: scale(1);
  transition: transform 0.3s;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #ff9595;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.3s;
}

.fade-enter,
.fade-leave-to{
  opacity:0;
  /* transform: translateX(-30%); */
}

.avatar {
  width: 100px;
  height: 100px;
  border-radius: 50%;
}

</style>

