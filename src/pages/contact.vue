<template>
  <div id="wrapper">
    <main id="content">
      
      <HelloWorld />
    </main>
    
  </div>
</template>

<style>
*,
html,
body {
  box-sizing: border-box;
}

html,
body {
  margin: 0;
  padding: 0;
}

:root {
  --primaryFont: Avenir, Helvetica, Arial, sans-serif;
}

#app {
  font-family: var(--primaryFont);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#content {
  flex: 1;
  margin-top: 30px;
}

#footer {
  padding: 30px;
}

#wrapper {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
}

a {
  color: #42b983;
}

button {
  padding: 8px 16px;
}
</style>
