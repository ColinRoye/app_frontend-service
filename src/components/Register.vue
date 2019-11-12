<template>
     <body>
     <div class="container">


      <div class="row">
          <form>
            <div class="row">

                <div class="col s12 m6 offset-m3">
                      <div class="card center-align mg">

                          <div class="card-content">
                              <h3>Register Profile</h3>
                              <div class="input-field">

                                  <input id="username" v-model="username" type="text" class="validate">
                                  <label for="username">Username</label>
                              </div>
                              <div class="input-field">

                                  <input id="email" v-model="username" type="text" class="validate">
                                  <label for="email">Email</label>
                              </div>
                              <div class="input-field" >
                                  <input id="password" v-model="password" type="password" class="validate">
                                  <label for="password">Password</label>

                              </div>
                              <button class="btn pulse blue lighten-1 waves-light" type="submit" v-on:click="register()" name="action">Register
                                  <i class="material-icons right">send</i>
                              </button>
                          </div>


                        </div>
                      </div>
                </div>


          </form>

      </div>
     </div>
     </body>
</template>

<script>
    export default {
        name: 'Register',
        data() {
            return {
                input: {
                    username: "",
                    password: ""
                }
            }
        },
        methods: {
            register() {


            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
     <style scoped>
     h3 {
       margin: 40px 0 0;
     }
     ul {
       list-style-type: none;
       padding: 0;
     }
     li {
       display: inline-block;
       margin: 0 10px;
     }
     a {
       color: #34ADFF;
     }
</style>
