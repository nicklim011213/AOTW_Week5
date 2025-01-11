<script setup lang="ts">
import ProjectTile from './components/Project.vue'
import './index.css'

const Projects = ([
  {Title: "Title1", Desc:"Desc1"},
  {Title: "Title2", Desc:"Desc2"},
  {Title: "Title3", Desc:"Desc3"},
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
      <ProjectTile v-bind="Projects[0]"></ProjectTile>
      </li>
      <li>
      <ProjectTile v-bind="Projects[1]"></ProjectTile>
      </li>
      <li>
      <ProjectTile v-bind="Projects[2]"></ProjectTile>
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
    margin-left: 85%;
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
