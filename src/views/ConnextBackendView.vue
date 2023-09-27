<template>
    <v-container>
      <v-row>
        <v-col cols="12">
              <ConnextBackend/>
        </v-col>
      </v-row>
    </v-container>
  
  </template>
  
  <script>
  export default {
      components:{
        ConnextBackend:() => import('../components/ConnextBackend.vue')
      }
      
  }
  </script>
  
  <style>
  
  </style>
