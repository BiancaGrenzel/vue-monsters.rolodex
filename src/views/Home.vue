<template>
  <div class="home">
    <div>
      <CardComponent></CardComponent>
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
    fetch
      .get("https://jsonplaceholder.typicode.com/users")
      .then((res) => res.json())
      .then((users) => (this.monsters = users));
  },
};
</script>

<script></script>
