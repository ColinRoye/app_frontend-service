<template>
     <body>

       <div class="row">
         <div class="col s12 m3">
           <div class="card horizontal">
             <div class="card-image">
               <img class="responsive-img" src="./../assets/defaultUser.jpg" />
             </div>
             <div class="card-stacked">
               <div class="card-content">
                 <p> {{username}}</p>
               </div>
               <div class="card-action">
                 <button class="btn pulse blue lighten-1 waves-light" type="submit" v-on:click="follow()" name="action">Follow</i>
                 </button>
               </div>
               </div>
             </div>
           </div>
         </div>

     </body>
</template>

<script>
    export default {
        name: 'Login',
        data() {
            return {
                input: {
                    username: "",
                    password: ""
                }
            }
        },
        methods: {
            login() {
                // let ret = axios.post("http://hackguy.cse356.compas.cs.stonybrook.edu/login",{
                  // username:
                  // password:
                // })
                if(this.input.username != "" && this.input.password != "") {
                    if(this.input.username == this.$parent.mockAccount.username && this.input.password == this.$parent.mockAccount.password) {
                        // this.$emit("authenticated", true);
                        // this.$router.replace({ name: "secure" });
                        alert("Hello! I am an alert box!!");

                    } else {
                        // console.log("The username and / or password is incorrect");
                    }
                } else {
                    // console.log("A username and password must be present");
                }
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
     <style scoped>
     .row {
       /* position: relative;

        width:1200px;
        max-height:160px; */
      }
    .test {
       border-radius: 50%;

     }
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
