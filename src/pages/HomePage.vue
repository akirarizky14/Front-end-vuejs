<template>
  <div class="home-page">
    <h1 class="todo">To-Do List</h1>
    <img src="https://sun9-27.userapi.com/impg/c857432/v857432393/179497/Aqu-55jn2jQ.jpg?size=1440x2160&quality=96&sign=a1f679b2e8c792cd1db7c19cacfc33d5&type=album" width="50%"/>
    <h2>Akira Rizky // BSBO 06 19</h2>
  </div>
</template>

<script>
export default {
  name: "HomePage",
  async created() {
    const response = await fetch("https://jsonplaceholder.typicode.com/todos");
    console.warn({ response });
  },
};
</script>

<style></style>
