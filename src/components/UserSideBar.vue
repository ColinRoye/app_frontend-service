<template>
  <body>
    <h1>test</h1>
    <ul >
      <li v-for="message in messages"> test{{message}}</li>

    </ul>
  </body>

</template>

<script>
    export default {
        name: 'UserSideBar',
        data() {
          return {
            messages:  ['hello', 'vue', 'js'],
            shoppingItems: [
              {name: 'apple', price: '10'},
              {name: 'orange', price: '12'}
            ]
          }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
