<template>

   <div class="columns is-mobile is-centered">
     <div class="column is-3">
       <section class="section" v-for="(info, key) in cardInfo">
       <card :info="info" :index="key" ></card>
       </section>
     </div>
   </div>

</template>

<script>

import Card from "../components/Card";

export default {
  components: {Card},
  data(){
    return {
      cardInfo: [
        {
          name: 'Risto Valge',
          image: 'https://picsum.photos/1280/960/?random',
          userImage: 'https://picsum.photos/96/96/?random'
        },
        {
          name: 'Kalle Muus',
          image: 'https://picsum.photos/1280/960/?random',
          userImage: 'https://picsum.photos/96/96/?random'
        },
        {
          name: 'Mart Läts',
          image: 'https://picsum.photos/1280/960/?random',
          userImage: 'https://picsum.photos/96/96/?random'
        },
        {
          name: 'Kaidi Pisike',
          image: 'https://picsum.photos/1280/960/?random',
          userImage: 'https://picsum.photos/96/96/?random'
        }
      ]
    }


  },

  computed: {}
}

</script>

<style>

</style>
