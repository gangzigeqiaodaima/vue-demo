<template>
  <div class="home">
    <div class="page-top">
      页面顶部
    </div>
    <div class="page-nav">
      <ul>
        <li><router-link to="/demoList">demoList</router-link></li>
      </ul>
    </div>
    <div class="page-content">
      <router-view/>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    // HelloWorld
  },
  methods: {
  }
}
</script>
<style scoped lang="scss">
  div.home {
    width: 100%;
    height: 100%;
    position: relative;
    div.page-top {
      width: 100%;
      height: 120px;
      background-color: #23262F;
      color: #ffffff;
    }
    div.page-nav {
      position: absolute;
      left: 0px;
      top: 120px;
      bottom: 0px;
      width: 300px;
      background-color: #393D49;
      color: #ffffff;
      ul {
        list-style-type: none;
        color: #ffffff;
        padding: 0px;
        margin: 0px;
        a {
          color: #ffffff;
        }
      }
    }
    div.page-content {
      position: absolute;
      left: 300px;
      top: 120px;
      bottom: 0px;
      right: 0px;
    }
  }
</style>
