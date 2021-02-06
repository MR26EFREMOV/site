<template>
  <div>
    <section>
      <v-container>
        <v-row>
          <v-col class="py-5">
            <h1>{{ header }}</h1>
          </v-col>
        </v-row>
      </v-container>
    </section>
    <section v-for="block in blocks" :key="block.id" class="section">
      <v-container>
        <v-row>
          <v-col cols="12" md="9">
            <h2>
              {{ block.title }}
            </h2>
            <v-list>
              <v-list-item v-for="row in block.textRows" :key="row"
                >{{ row }}
              </v-list-item>
            </v-list>
          </v-col>
          <v-col cols="12" md="3">
            <img :src="block.image" class="logo" alt="" />
          </v-col>
        </v-row>
      </v-container>
    </section>
    <section>
      <v-container>
        <v-row>
          <v-col
            ><p>Заитересовала одна из услуг?</p>
            <p>
              Вы можете связаться с нами по номеру
              <a href="tel:43343">43434343434</a>
            </p>
          </v-col>
        </v-row>
      </v-container>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Main',
  data() {
    return {
      header: 'Консультации по ГИС, ArcGIS, QGIS, ДЗЗ',
      blocks: [
        {
          textRows: [
            'Консультирование по программе ArcGIS',
            'Помощь в организации рабочих процессов',
            'Разработка дополнительных инструментов для работы ',
          ],
          image: 'img/logo_1.png',
          title: 'заголовок',
          id: '1',
        },
        {
          textRows: [
            'Консультирование по программе ArcGIS',
            'Помощь в организации рабочих процессов',
            'Разработка дополнительных инструментов для работы ',
          ],
          image: 'img/logo_1.png',
          title: 'заголовок',
          id: '2',
        },
        {
          textRows: [
            'Консультирование по программе ArcGIS',
            'Помощь в организации рабочих процессов',
            'Разработка дополнительных инструментов для работы ',
          ],
          image: 'img/logo_1.png',
          title: 'заголовок',
          id: '3',
        },
      ],
    }
  },
}
</script>
