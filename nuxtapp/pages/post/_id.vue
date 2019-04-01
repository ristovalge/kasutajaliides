<template>
    <div>
      {{$route.params.id}}
    </div>
</template>

<script>
    export default {
        name: "_id",

        validate ({ params }) {
          // Must be a number
          return /^\d+$/.test(params.id)
        }

    }
</script>

<style scoped>

</style>
