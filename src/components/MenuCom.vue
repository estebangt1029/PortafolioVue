<template>
    <nav>
        <RouterLink class="btn third" to="/">Home</RouterLink>
        <RouterLink class="btn third" to="/projects">Projects</RouterLink>
        <RouterLink class="btn third" to="/about">About</RouterLink>
    </nav>
</template>

<style scoped>
nav {
    position: fixed;
    top: -10px;
    right: 5px;
    height: 10vh;
    display: flex;
    gap: 10px;
    justify-content: space-evenly;
    align-items: center;
    font-size: xx-large;  
    z-index: 1;
}
a{
    text-decoration: none;
    color: #ffff51;
    padding: 5px;
}
.btn {
  border: 2px solid #e74c3c;
  border-radius: 0.6em;
  cursor: pointer;
  font-size: 1rem;
  line-height: 1;
  padding: 10px;
  font-family: 'Montserrat', sans-serif;
  text-decoration: none;
    color: #ffff51;
}
.btn:hover, .btn:focus {
  color: #fff;
  outline: 0;
}
.third {
  border-color: #e74c3c;
  color: #fff;
  -webkit-transition: all 150ms ease-in-out;
  transition: all 150ms ease-in-out;
}
.third:hover {
  background-color: #e74c3c;
}
</style>








