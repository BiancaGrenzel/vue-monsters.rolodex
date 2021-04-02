<template>
  <div class="home">
    <div class="card-list">
      <CardComponent v-for="monster in monsters" v-bind:key="monster.id" :monster="monster"></CardComponent>
    </div>
    <!-- <CardList></CardList>
    <SearchBox></SearchBox> -->
  </div>
</template>

<script>
// @ is an alias to /src
import CardComponent from "@/components/card/Card.component.vue";
// import CardList from "@/components/card-list/CardList.component.vue";
// import SearchBox from "@/components/search-box/SearchBox.component.vue";

export default {
  name: "Home",
  components: {
    'CardComponent':CardComponent
  },

  data() {
    return {
      monsters: [],
    };
  },

  created() {
      fetch("https://jsonplaceholder.typicode.com/users")
      .then(res => res.json())
      .then((users) => (this.monsters = users));
  },
};
</script>

<style>
.card-list {
    width: 85vw;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-gap: 20px;
  }
  
</style>

