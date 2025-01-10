<script setup lang="ts">
import ProjectTile from './components/Project.vue'
import './index.css'
</script>

<template>
    <div id="TopBar"></div>
    <h1> Current Projects:</h1>
    <ul>
      <li>
      <ProjectTile></ProjectTile>
      </li>
      <li>
      <ProjectTile></ProjectTile>
      </li>
      <li>
      <ProjectTile></ProjectTile>
      </li>
    </ul>
</template>

<style scoped>
li
{
  list-style: none;
}

ul
{
  padding-left: 0%;

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
  width: 100vw;
  height: 5vh;
  background-color: #00aeff;
}

h1
{
  text-align: center;
  align-self: center;
  margin: 2%;
}
</style>
