<template>
  <v-footer>
    <v-container>
      <v-row justify="center">
        <v-col v-for="btn in btns" :key="btn.id" class="_center">
          <v-btn :href="btn.href">
            <v-icon size="24px">
              {{ btn.icon }}
            </v-icon>
          </v-btn>
        </v-col>
      </v-row>
      <v-divider></v-divider>
      <v-row>
        <v-card-text class="white--text">
          <v-col class="_center">
            {{ new Date().getFullYear() }} —
            <strong>ГИС-Консультирование</strong>
          </v-col>
        </v-card-text>
      </v-row>
    </v-container>
  </v-footer>
</template>

<script>
export default {
  name: 'Footer',
  data() {
    return {
      btns: [
        {
          id: 1,
          icon: 'mdi-phone',
          color: 'dark',
          href: 'tel:+3322323232323',
        },
        {
          id: 2,
          icon: 'mdi-account-group',
          color: 'dark',
          href: 'http://gis.psu.ru/',
        },
        {
          id: 3,
          icon: 'mdi-email',
          color: 'dark',
          href: 'mailto:someemail',
        },
      ],
    }
  },
}
</script>
