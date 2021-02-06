<template>
  <v-container>
    <v-row>
      <v-tabs class="_center">
        <v-tab v-for="route in routes" :key="route.id" :to="route.route">{{
          route.name
        }}</v-tab>
      </v-tabs>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'NavBar',
  data() {
    return {
      routes: [
        {
          id: '1',
          route: '/',
          name: 'Главная',
        },
        {
          id: '2',
          route: '/about',
          name: 'Про нас',
        },
        {
          id: '3',
          route: '/contacts',
          name: 'Контакты',
        },
      ],
    }
  },
}
</script>
