<template>
  <v-app id="app">
      <v-navigation-drawer
        color="green"
        dark
        expand-on-hover
        hide-overlay
        permanent
        right
        app
      >
        <v-list
          nav 
          shaped
          dense
        >
          <v-list-item>
            <v-list-item-avatar>
              <img :src=" 'https://randomuser.me/api/portraits/men/1.jpg' ">
            </v-list-item-avatar>

            <v-list-item-content>
              <v-list-item-title class="font-weight-black">SocialLink</v-list-item-title>
              <v-list-item-subtitle>Иван Иванов</v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>

          <v-divider class="my-3"></v-divider>

          <v-list-item link :to="путь">
            <v-list-item-icon>
              <v-icon>mdi-home-outline</v-icon>
            </v-list-item-icon>

            <v-list-item-content>
              <v-list-item-title class="text-left">Главная</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          <v-list-item link :to="путь">
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>

            <v-list-item-content>
              <v-list-item-title class="text-left">Мой профиль</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          <v-list-item link :to="путь">
            <v-list-item-icon>
              <v-icon>mdi-account-multiple-plus</v-icon>
            </v-list-item-icon>

            <v-list-item-content>
              <v-list-item-title class="text-left">Найти друзей</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
    
    <v-content class="px-12 py-3">
      <v-container fluid>
        <router-view/>
      </v-container>
    </v-content>

  </v-app>
</template>

<script>
export default {
  name: 'App',

  components: {
  },

  data: () =>({
    //
  }),
};
</script>
