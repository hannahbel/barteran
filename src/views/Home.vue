<template>
  <v-app>
    <v-main>
      <v-container fluid>
        <v-row align="center" justify="center">
          <v-col cols="12" sm="8" md="8">
            <v-card class="elevation-12">
              <v-window v-model="step">
                 <v-window-item :value="1">
                   <v-row>
                     <v-col cols="12" md="8">
                       <v-card-text class="mt-12">
                         <h1 class="text-center display-2 grey--text text--darken-2">Welcome back.</h1>
                         <h4 class="text-center mlt-4 grey--text text--darken-1">Ready for another round of trades?</h4>
                         <v-form>
                           <v-text-field
                             label="Username"
                             name="Username"
                             prepend-icon="person"
                             type="text"
                             color="deep-orange lighten-3" />
                          <v-text-field
                          id="password"
                          label="Password"
                          name="Password"
                          prepend-icon="lock"
                          type="password"
                          color="deep-orange lighten-3" />
                         </v-form>
                         <h3 class="text-left mt-3"><a href="#">Forgot password?</a></h3>
                       </v-card-text>
                       <div class="text-center mt-3">
                         <v-btn to="/dashboard" rounded color="green accent-3" dark>SIGN IN</v-btn>
                       </div>
                     </v-col>
                       <v-col cols="12" md="4" class="red lighten-2">
                       <v-card-text class="white--text mt-12">
                         <h1 class="text-center display-1">No account?</h1>
                         <h4 class="text-center">Join Barteran today for free.</h4>
                       </v-card-text>
                       <div class="text-center">
                         <v-btn rounded outlined="" dark @click="step++">REGISTER</v-btn>
                         </div>
                         </v-col>
                   </v-row>

                </v-window-item>
                 <v-window-item :value="2">
                   <v-row class="fill-height">
                     <v-col cols="12" md="4" class="red lighten-2">
                       <v-card-text class="white--text mt-12">
                         <h1 class="text-center display-1">Already joined?</h1>
                         <h5 class="text-center">Log back in and don't miss out!</h5>
                       </v-card-text>
                       <div class="text-center">
                         <v-btn rounded outlined="" dark @click="step--">LOG IN</v-btn>
                       </div>
                     </v-col>
                     <v-col cols="12" md="8">
                       <v-card-text class="mt-12">
                         <h1 class="text-center display-2 grey--text text--darken-2">Welcome Aboard!</h1>
                         <h4 class="text-center mt-4 grey--text text--darken-1">Be part of the growing trade community.</h4>
                         <v-form>
                           <v-text-field
                           label="First Name"
                           name="Firstname"
                           prepend-icon="person"
                           type="text"
                           color="deep-orange lighten-3" />
                           <v-text-field
                           label="Last Name"
                           name="Lastname"
                           prepend-icon="person"
                           type="text"
                           color="deep-orange lighten-3" />
                           <v-text-field
                           label="Contact No."
                           name="ContactNo"
                           prepend-icon="phone"
                           type="text"
                           color="deep-orange lighten-3" />
                           <v-text-field
                           label="Current Address"
                           name="Address"
                           prepend-icon="house"
                           type="text"
                           color="deep-orange lighten-3" />
                           <v-text-field
                           label="Email"
                           name="Email"
                           prepend-icon="email"
                           type="text"
                           color="deep-orange lighten-3" />
                           <v-text-field
                           label="Password"
                           name="Password"
                           prepend-icon="lock"
                           type="password"
                           color="deep-orange lighten-3" />
                           <v-text-field
                           label="Re-enter Password"
                           name="Password2"
                           prepend-icon="lock"
                           type="password"
                           color="deep-orange lighten-3" />
                         </v-form>
                       </v-card-text>
                       <div class="text-center mt-n5">
                         <v-btn to="/dashboard" rounded color="green accent-3" dark>SIGN UP</v-btn>
                       </div>
                     </v-col>
                   </v-row>

                </v-window-item>
              </v-window>    
            </v-card>
          </v-col>
        </v-row>
      </v-container>

    </v-main>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    step: 1
  }),
  props: {
    source: String
  }
}
</script>