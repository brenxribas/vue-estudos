<template>
  <div>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Projetos</a></li>
      <li><a href="#">Contato</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
ul {
  list-style: none;
  display: flex;   
  justify-content: center;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
 
li {
  margin-right: 20px;
}

li a {
  color: white;
  text-decoration: none;
  transition: 0.5s;
}

li a:hover {
    color: aqua;
}
</style>