<template>
  <div>
    <section>
      <v-container>
        <v-row>
          <v-col class="py-5">
            <h1>{{ header }}</h1>
          </v-col>
        </v-row>
        <v-row>
          <v-col>
            <p>Номер - <a href="tel:43434">3433434</a></p>
            <p>Почта - <a href="mailto:someemail">gis.sdsf@df.ru</a></p>
          </v-col>
        </v-row>
      </v-container>
    </section>
    <section>
      <v-container>
        <v-row>
          <h1>Вы можете нас по адресу г.Пермь, ПГНИУ</h1>
          <v-col class="py-5">
            <YMap />
          </v-col>
        </v-row>
      </v-container>
    </section>
  </div>
</template>

<script>
import YMap from './YMap'

export default {
  name: 'Contacts',
  components: {
    YMap,
  },
  data() {
    return {
      header: 'Связаться с нами',
    }
  },
}
</script>
