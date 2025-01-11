<script setup>

defineProps(
    {
        Title: {type: String},
        Desc: {type: String}    
    }
)
</script>

<template>
    <h1 id="ProjectTitle"> {{ Title }}</h1>
    <p> {{ Desc }}</p>
</template>

<style scoped>

#ProjectTitle
{
    font-size: 2em;
    text-align: left;
}

</style>