<template>
  <div>
    <nav id="nav">
      <h1 class="title"><span class="pro"> Puzzle</span>Pro</h1>
      <ul class="links">
        <li>
          <router-link to="/">Accueil</router-link>
        </li>
        <li>
          <router-link to="/articles">Listes des articles</router-link>
        </li>
      </ul>
    </nav>
  </div>
</template>


<style >
#nav {
  background-color: black;
  color: white;
  display: flex;
  padding: 20px;
}

.pro {
  color: yellow;
}

.title {
  font-size: 25px;
  margin-left: 20px;
}

.links {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  margin-left: 40px;
}

a {
  color: white;
  text-decoration: none;
}

a:hover {
  color: yellow;
}

li {
  margin-left: 20px;
  list-style: none;
  font-size: 20px;
}

.main {
  background-color: gray;
}

@media screen and (max-width: 500px) {
  #nav {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .links {
    flex-direction: column;
    justify-content: flex-start;
    align-items: initial;
  }

  li {
    margin-left: 0px;
    margin: 5px 0px;
    border-bottom: 1px solid yellow;
    padding: 0 0 10px 0;
    text-align: center;
  }

  
}
</style>
