<template>
  <div>
    <input type="text" v-model="newTodoItem"><!-- v-model 의 역할 : input에 입력된 값을 동적으로 바로바로 vue instance 안에 매핑 -->
    <button v-on:click="addTodo">add</button>
  </div>
</template>

<script>
export default {
  data: function(){
    return {
      newTodoItem: ""
    }
  },
  methods: {
    addTodo: function(){
      // 저장하는 로직
      localStorage.setItem(this.newTodoItem, this.newTodoItem); // key, value 형태로 저장
      this.newTodoItem = '';
    }
  }
}
</script>

<style>

</style>