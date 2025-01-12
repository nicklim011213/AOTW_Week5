<script setup>

defineProps(
    {
        Title: {type: String},
        Desc: {type: String},
        ImgPath: {type: String}    
    }
)
</script>

<template>
    <div id="ProjectContiner">
        <h1 id="ProjectTitle"> {{ Title }}</h1>
        <p> {{ Desc }}</p>
        <img :src="ImgPath" />
    </div>
</template>

<style scoped>

#ProjectTitle
{
    font-size: 4em;
    text-align: left;
}

p
{
    max-width: 20vw;
}

img
{
    width: 20vw;
    height: 20vh;
}

#ProjectContiner
{
    width: 20vw;
    height: 20vh;
    text-align: left;
}

</style>