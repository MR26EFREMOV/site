<template>
  <no-ssr>
    <yandex-map :coords="coords" :zoom="zoom"> </yandex-map>
  </no-ssr>
</template>

<script>
import { yandexMap } from 'vue-yandex-maps'
export default {
  components: { yandexMap },
  data: () => ({
    coords: [58.007869, 56.186618],
    zoom: 15,
  }),
}
</script>
