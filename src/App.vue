<template>
  <div>
    <!-- <app-header v-bind:프롭스 속성 이름="상위 컴포넌트의 데이터 이름"></app-header> -->
    <app-header v-bind:propsdata="str"></app-header>
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
      str: 'Header'
    }
  },
  components: {
    'app-header': AppHeader
  }
}
</script>

<style>

</style>