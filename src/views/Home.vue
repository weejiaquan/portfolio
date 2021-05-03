<template>
  <div class="home page">
    <transition appear
    @before-enter="beforeEnter"
    @enter="enter"
>


    <div class="introduction">
    <h1>HELLO,</h1>
    <h2>I am Wee Jia Quan, a student in University of British Columbia with experience with System Administration / Web Development from Malaysia.</h2>
    <h3>I have rich experience in IT, Web Hosting and developing, scripting, and reimaging machines in production environment.</h3>
</div>
    </transition>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import gsap from "gsap";





export default {
  name: "Home",
  created(){
    console.log("tf");
  },
  components: {
    HelloWorld,
  },
};
</script>
