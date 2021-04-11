<template>
  <div>
    <app-header></app-header>
  </div>
</template>

<script>
// AppHeader.vue를 App.vue에서 사용하기 위해 import 
// AppHeader.vue 파일이 AppHeader 변수명에 저장
import AppHeader from './components/AppHeader.vue';

// var AppHeader = {
//   template: '<header><h1>Header</h1></header>';
// }

// new Vue({
//   data: {
//     str: 'hi'
//   }
// })

export default {
  data: function() {
    return {
      str: 'hi'
    }
  },
  components: {
    'app-header': AppHeader
  }
}
</script>

<style>

</style>