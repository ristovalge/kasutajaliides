<template>

<post-list :posts="posts"></post-list>
</template>

<script>


import PostList from "../components/postList";
var faker = require('faker');
export default {
  components: {PostList},
  data(){
    return {
      posts: [
        {id: faker.random.number(100), content: faker.lorem.paragraph(10), title:faker.lorem.sentence(10, 8)},
        {id: faker.random.number(100), content: faker.lorem.paragraph(50), title:faker.lorem.sentence(10, 8)},
    ]
    }
  }
}



</script>

<style lang="scss">
 /* .button.one {
    background-color: crimson;
  }
  .button.two {
    background-color: orangered;
  }
  .button.three {
    background-color: #35495e ;
  }
*/
input{
  background-color: $primary !important;
}

</style>
