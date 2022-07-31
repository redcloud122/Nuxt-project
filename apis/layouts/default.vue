<template>
  <div>
    <header>
      <img src="~/assets/ContosoCompanyLogo.jpg" alt="Logo" width="100" />
      <h1>The Contoso Company</h1>
    </header>

    <nav>
      <div>
        <nuxt-link to="/">Home</nuxt-link>
        <nuxt-link to="/image">Image</nuxt-link>
        <nuxt-link to="/accordion">Accordion</nuxt-link>
        <nuxt-link to="/grid">Grid</nuxt-link>
      </div>
    </nav>

    <nuxt/>
    <footer><p>Footer</p></footer>
  </div>
</template>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
}

header img {
  max-width: 50%;
}

header h1 {
  margin: 0;
  padding: 2rem 0;
  text-align: center;
  font-weight: 400;
  color: #0033A1;
}

nav {
  background: #f8f9fa;
  padding: 18px 18px 18px 0;
  display: flex;
  justify-content: space-between;
}

nav div {
  padding-right: 2rem;
}

nav a {
  padding: 20px;
  color: rgba(0,0,0,.5);
  text-decoration: none;
  transition: .7s;
}

nav a:hover {
  background-color: rgba(132, 210, 236, 0.429);
  color: #0033A1;
}

a.nuxt-link-exact-active {
  color: #0033A1;
}

footer{
  background: rgb(155, 153, 153);;
  text-align: center;
  vertical-align: middle;
  color: white;
  height: 100px;
  padding-top: 34px;
}


</style>

