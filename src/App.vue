<template>
  <div id="app">
    <Header />
    <Todos v-bind:todos="[]" v-on:del-todo="deleteTodo"/>
    <Body />
  </div>
</template>

<script>
import Header from './components/layout/Header';
import Body from './components/layout/Body';
import Todos from './components/Todos';


export default {
  name: 'App',
  components: {
      Header,
      Todos,
      Body
  },
  methods: {
    deleteTodo(id) {
      this.todos = this.todos.filter(todo => todo.id !== id);
      },
    }
}
</script>

<style>
 * {
   box-sizing: border-box;
   margin: 0%;
   padding: 0%;
 }

  body {
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.4;
  }

  .btn {
    display: inline-block;
    border: none;
    background: #555;
    color: #fff;
    padding: 7px 20px;
    cursor: pointer;
  }

  .btn:hover{
    background: #666;
  }
</style>
