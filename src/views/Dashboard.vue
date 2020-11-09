<template>
 <v-app>
     <v-navigation-drawer v-model="drawer" dark app mini-variant class="red lighten-2">
                        <v-list flat>
                            <v-list-item class="mb=12">
                                <v-list-item-action>
                                    <v-icon>fas fa-cloud-download-alt</v-icon>
                                </v-list-item-action>
                            </v-list-item>
                            <v-list-item router to="/">
                                <v-list-item-action>
                                    <v-icon>fas fa-desktop</v-icon>
                                </v-list-item-action>
                            </v-list-item>
                       <v-list-item router to="/">
                                <v-list-item-action>
                                        <v-badge color="yellow">    
                                         <template v-slot:badge>1</template>
                                    <v-icon>fas fa-shopping-cart</v-icon>
                                        </v-badge>
                                </v-list-item-action>
                            </v-list-item>
                            <v-list-item router to="/">
                                <v-list-item-action>
                                    <v-icon>fas fa-city</v-icon>
                                </v-list-item-action>
                            </v-list-item>
                             <v-list-item router to="/">
                                <v-list-item-action>
                                    <v-icon>fas fa-cog</v-icon>
                                </v-list-item-action>
                            </v-list-item>
                        </v-list>
                    </v-navigation-drawer>
           
               <v-container>
                   <v-row>
                       <v-col cols="12" md="4">
                           <v-text-field label="Search items" prepend-icon="search" color="red" error></v-text-field>
                       </v-col>
                       <v-spacer></v-spacer>
                       <v-btn text class="mt-7">
                           <v-icon color="red" class="mr-n10">menu</v-icon>
                       </v-btn>
                       <v-btn text class="mt-7">
                           <v-icon color="red" class="mr-n10">dashboard</v-icon>
                       </v-btn>
                   </v-row>
               </v-container>
            </v-app>
</template>

<script>
export default {
    name: 'dashboard',

    data: ()=>({
        drawer: true
    })
}
</script>