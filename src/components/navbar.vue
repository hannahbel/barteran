<template>
    <nav>
        
            <v-app-bar app class="text-uppercase" color="white">  
                <v-toolbar-title>
                    <span class="font-weight-light red--text text--lighten-2">Nikol</span>
                    <span class="red--text text--lighten-1">Barteran</span>
                    </v-toolbar-title>
                    <div class="flex-grow-1"></div>
                     <v-btn to="/" text color="grey darken-1" href="#" target="_blank">
                            <span class="mr-2">Sign In</span>
                     </v-btn>
                    <v-btn text color="grey darken-1" href="#" target="_blank">
                            <span class="mr-2">Log Out</span>
                            <v-icon color="grey darken-1" >mdi-logout</v-icon>
                        </v-btn>    
                    </v-app-bar>
                 
                
    </nav>
</template>

<script>
export default {
    
    data: ()=>({
        drawer: true
    })
}
</script>