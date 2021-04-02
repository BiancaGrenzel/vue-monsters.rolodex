<template>

    <div class="card-container">
        <img class="icon" :src="`https://robohash.org/${monster.id}?set=set2&size=180x180`" alt="monster">
        <h1>{{ monster.name }}</h1>
        <p>{{ monster.email }}</p>
        <!-- <h1>{{ monster.name }}</h1>
        <p>{{ monster.email }}</p> -->
    </div>
   
</template>
<script>

export default{
    // props:['monster']
    name:"CardComponent",
    props:{
        monster:Object
    }
}

</script>

<style lang="sass" scoped>
@import "./Card.styles.scss";
</style>