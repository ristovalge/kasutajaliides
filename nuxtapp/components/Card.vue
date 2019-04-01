<template>
  <div class="card">
    <div class="card-image">
      <figure class="image is-4by3">
        <img :src="info.image + '&key=' + index" alt="Placeholder image">
      </figure>
    </div>
    <div class="card-content">
      <div class="media">
        <div class="media-left">
          <figure class="image is-48x48">
            <img :src="info.userImage + '&key=' + index" alt="Placeholder image">
          </figure>
        </div>
        <div class="media-content">
          <p class="title is-4">{{info.name}}</p>
          <p class="subtitle is-6">@{{nameTag}}</p>
        </div>
      </div>

      <div class="content">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit.
        Phasellus nec iaculis mauris. <a>@bulmaio</a>.
        <a href="#">#css</a> <a href="#">#responsive</a>
        <br>
        <time>{{currentDate}}</time>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        name: "Card",
      props: ['info', 'index'],
      computed: {
          nameTag(){
            return this.info.name.replace(' ','').toLowerCase();
          },
        currentDate(){
            let date = new Date();
            return date.toDateString()
        }
      }
    }
</script>

<style scoped>

</style>
