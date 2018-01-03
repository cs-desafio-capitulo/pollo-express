<template>
  <div class="hello">
    <md-app md-mode="fixed">
      <md-app-toolbar class="md-primary">
        <md-button @click="menuVisible = !menuVisible">Button</md-button>
        <span class="md-title">Pollo-express</span>
      </md-app-toolbar>

      <md-app-drawer :md-active.sync="menuVisible">
        <md-toolbar class="md-transparent" md-elevation="0">
          Menu
        </md-toolbar>

        <md-list>

          <md-list-item>
            <span>Login</span>
          </md-list-item>

          <md-list-item>
            <span>Stuff</span>
          </md-list-item>

          <md-list-item>
            <span>Stuff2</span>
          </md-list-item>

          <md-list-item>
            <span>Stuff3</span>
          </md-list-item>

        </md-list>
      </md-app-drawer>
    </md-app>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: () => ({
    menuVisible: false,
  }),
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
