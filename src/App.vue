<template>
  <v-app>
    <v-app-bar
      app
      color="dark"
      dark
    >
      <!-- <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div> -->

      <v-spacer></v-spacer>
      <v-btn
        text
        @click="goToHome()"
      >
      Connext Backend
      
      </v-btn>
      <v-btn
        text
        @click="goToManage()"
      >
        หน้าจัดการข้อมูล
      </v-btn>
      <v-btn
        text
        @click="goToLogin()"
      >
        เข้าสู่ระบบ
      </v-btn>
      <v-btn
        text
        @click="goToLogin()"
      >
        ออกจากระบบ
      </v-btn>
      
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>
  export default {
    name: 'App',
    data: () => ({
    }),
  
    methods: {
      goToLogin(){
        this.$router.push('/')
      },
      goToManage(){
        this.$router.push('/ManageTable')
      },
      goToHome(){
        this.$router.push('/home')
      }

    }
  }
  </script>
  
  <style>
  
  </style>