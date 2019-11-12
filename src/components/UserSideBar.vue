<template>
  <div class="row">
    <div class="hl">

      <div class="col s12 m4 l4">
        <div class="card horizontal">
           <div class="card-content">
            <ul>
              <li v-for="message in messages">
                 <UserCard :username="message"></UserCard>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<script>
    import UserCard from './UserCard'
    export default {
        name: 'UserSideBar',
        components: {
          UserCard
        },
        data() {
          return {
            messages:  ['hello', 'vue', 'js','asdf'],
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
  .hl{
    max-width: 1115px;
  }
</style>
