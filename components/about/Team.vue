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
    <section v-for="member in members" :key="member.title" class="section">
      <v-container>
        <v-row>
          <v-col cols="12" md="9">
            <h2>
              {{ member.title }}
            </h2>
            <v-list>
              <v-list-item v-for="row in member.textRows" :key="row"
                >{{ row }}
              </v-list-item>
            </v-list>
          </v-col>
          <v-col cols="12" md="3">
            <img :src="member.image" class="logo" alt="" />
          </v-col>
        </v-row>
      </v-container>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Team',
  data() {
    return {
      header: 'Наша команда',
      members: [
        {
          textRows: [
            'Тут достойнство',
            'Тут описание',
            'Здесь еще что-то хорошее',
          ],
          image: 'img/logo_1.png',
          title: 'Фамилия имя',
        },
        {
          textRows: [
            'Консультирование по программе ArcGIS',
            'Помощь в организации рабочих процессов',
            'Разработка дополнительных инструментов для работы ',
          ],
          image: 'img/logo_1.png',
          title: 'Еще Имя фамиля',
        },
        {
          textRows: [
            'Консультирование по программе ArcGIS',
            'Помощь в организации рабочих процессов',
            'Разработка дополнительных инструментов для работы ',
          ],
          image: 'img/logo_1.png',
          title: 'и еще раз имя и фамилия',
        },
      ],
    }
  },
}
</script>
