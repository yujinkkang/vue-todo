<template>
  <div id="app">
    
  </div>
</template>

<script>
import TodoHeader from './components/TodoHeader.vue';
import TodoInput from './components/TodoInput.vue';
import TodoList from './components/TodoList.vue';
import TodoFooter from './components/TodoFooter.vue';

var my_cmp = {
  template: '<div>my component</div>'
}

new Vue({
  el: '',
  components:{
    'my-cmp': my_cmp
  }
})

export default {

}
</script>

<style>

</style>
