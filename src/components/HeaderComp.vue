<template>
  <header>
    <span class="logo"
      ><RouterLink to="/" class="titulo"> Crelo </RouterLink></span
    >
    <span><RouterLink to="/" class="botão"> Home </RouterLink></span>
    <span> | </span>
    <span><RouterLink to="/conta" class="botão"> Conta </RouterLink></span>
  </header>
</template>
<style scoped>
header {
  background-color: #f5b5bb;
  padding: 1%;
}
header span {
  color: black;
  font-size: larger;
  margin: 3px;
}

header a.botão {
  text-decoration: none;
  display: inline-block;
  transition: 0.25s;
  color: black;
}

header a.botão:hover {
  transform: scale(1.1) rotate(5deg);
}

header a.titulo {
  text-decoration: none;
  color: black;
}

span.logo {
  font-size: 200%;
  margin: 10px;
  font-weight: bolder;
}
</style>
