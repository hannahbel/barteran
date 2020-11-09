<template>

  <v-app>
    <v-main>
      <navbar />
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<style scoped>
.theme--light.v-application
{
    background: #f5f3f3;
     
}
</style>



<script>
import navbar from '@/components/navbar'

export default {
  name: 'App',

  components: { navbar },

  data: () => ({
      drawer: true
  }),
};
</script>
