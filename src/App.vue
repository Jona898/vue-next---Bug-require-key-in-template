<template>
  <div id="app">
    <ul>
      <template v-for="todo in todos">
        <li :key="todo.text">{{ todo.text }}</li>
      </template>
    </ul>
  </div>
</template>

<script>
export default {
  name: "App",
  data: () => {
    return {
      todos: [
        { text: "Learn JavaScript", done: false },
        { text: "Learn Vue", done: false },
        { text: "Build something awesome", done: true },
      ],
    };
  },
};
</script>
