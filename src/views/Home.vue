<template>
  <div class="home">
      <div class="container">
        <header class="header">
          <div class="title">
            <h1>Kathie</h1>
          </div>
          <div class="headNav flex justify-between align-center">
            <div class="leftNav">
              <router-link to="/index">Home</router-link>
              <router-link to="/Archives">Archives</router-link>
            </div>
            <div class="rigthNav">
              <span class="iconfont icon-wifi1"></span>
              <span class="iconfont icon-seekicon"></span>
            </div>
          </div>
          
        </header>
        <section>
          <router-view/>
        </section>
      </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    // HelloWorld
  }
}
</script>
<style lang="scss">
  .header{
    width: 100%;
    height: 300px;
    background: #bbb;
    position: relative;
  }
  .headNav{
    padding: 15px 30px;
    a{
      color: #fff;
      text-shadow: 0 1px rgba(0,0,0,0.2);
      opacity: 0.6;
      margin-right: 15px;
      &:hover{
        opacity: 1;
      }
    }
    span{
      margin-left: 15px;
      font-size: 16px;
    }
  }
  .title{
    width: 100%;
    text-align: center;
    color: #fff;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
  }
</style>
