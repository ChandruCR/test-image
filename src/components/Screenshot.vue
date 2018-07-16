<template>
  <v-app>
    <v-layout row wrap>
      <v-flex v-for="i in 8" :key="`4${i}`" sm6 md4 lg3>
        <v-card dark color="primary">
          <v-card-media
            :src="'http://xx.xx.xx.xx/TestSpace/' + i + '/ScreenShot?' + new Date().getTime()" 
            height="300px"/>
          <v-card-title primary-title>
            http://xx.xx.xx.xx/TestSpace/{{i}}/Screenshot
          </v-card-title>
        </v-card>
      </v-flex>
      <v-flex>
          <v-card dark color="primary">

          </v-card>
      </v-flex>
    </v-layout>
  </v-app>
</template>

<script>
export default {
  name: "Screenshot"
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.screenshot {
  width: 100%;
  height: 300px;
}
</style>
