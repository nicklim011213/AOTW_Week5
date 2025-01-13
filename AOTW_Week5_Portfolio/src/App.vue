<script setup lang="ts">
import Project from './components/Project.vue'
import './index.css'

const Projects = ([
  {Title: "Floorspaces", Desc:"Floorspaces is a web app using Unity .Net servers and cloud staorge to draw save and render 3d spaces onto a lve website", ImgPath: "Floorspaces.gif"},
  {Title: "AOTW", Desc:"AOTW or App of The Week is a reoccuring series on my github that has me create a new app every week such as a p2p chat, graphics engine, or even this very website", ImgPath: "AOTW_Week2.png"},
  {Title: "C# Graphics Engine", Desc:"This project uses c# and SFML in order to simulate what a 3d view would look like given a 2d array as a map you can traverse. It uses custom renderers to read the array and draw the view", ImgPath: "2DProj.png"},
  ])
</script>

<template>
  <div id="Container">
    <div id="TopBar"></div>
    <div id="Banner">
      <h1> Current Projects:</h1>
      <img src="./assets/LimGEDemo.gif">
    </div>  
    <ul>
      <li>
      <Project v-bind="Projects[0]"></Project>
      </li>
      <li>
      <Project v-bind="Projects[1]"></Project>
      </li>
      <li>
      <Project v-bind="Projects[2]"></Project>
      </li>
    </ul>  
  </div>
</template>

<style scoped>
li
{
  list-style: none;
}

ul
{
  padding-left: 0%;
  background-color: lightgray;
  display: flex;
  flex-direction: column;
  height: 75%;

  li:nth-child(even)
  {
    margin-left: 5%;
    margin-top: 10%;
  }

  li:nth-child(odd)
  {
    margin-left: 75%;
    margin-top: 10%;
  }
}

#TopBar
{
  width: 100%;
  height: 2.5%;
  background-color: #00aeff;
}

h1
{
  position: absolute;
  margin-left: auto;
  margin-right: auto;
  left: 0;
  right: 0;
  text-align: center;
  padding-top: 5%;
}

img
{
  width: 100%;
  height: 100%;
}

#Container
{
  height: 100%;
  width: 100%;
}

#Banner
{
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 22.5%;
}
</style>
