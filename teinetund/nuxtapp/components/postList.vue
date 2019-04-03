<template>
    <div>
      <post v-for="post in posts" :key="post.id" :post="post"></post>

    </div>
</template>

<script>
    import Post from "./post";
    export default {
        name: "postList",
      components: {Post},
      props: ['posts']
    }
</script>

<style scoped>

</style>
