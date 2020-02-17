<template>
  <div class="home">
      <div class="container">
        <!-- 头部 -->
        <header class="header">
          <div class="title">
            <h1>Kathie</h1>
          </div>
          <div class="head-nav flex justify-between align-center">
            <div class="leftNav">
              <router-link to="/index">Home</router-link>
              <router-link to="/Archives">Archives</router-link>
            </div>
            <div class="right-nav flex align-center">
              <div>
               <span class="iconfont icon-wifi pointer"></span>
              </div>
              <div>
                <input type="text" class="srch-inp">
                <span class="iconfont icon-seekicon srch-icon"></span>
              </div>
            </div>
          </div>
          
        </header>
        <!-- 主体 -->
        <div class="outer flex">
          <section class="main">
              <router-view></router-view>
          </section>
          <aside class="list">
            <List tag="archives"/>
            <List tag="recent post"/>
          </aside>
        </div>
      </div>
  </div>
</template>

<script>
// @ is an alias to /src
import List from '@/components/List.vue'

export default {
  name: 'Home',
  components: {
    List
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
  .head-nav{
    padding: 15px 30px;
    a{
      color: #fff;
      text-shadow: 0 1px rgba(0,0,0,0.2);
      opacity: 0.6;
      margin-right: 20px;
      &:hover{
        opacity: 1;
      }
    }
    .right-nav{
      div:nth-of-type(1){
        margin-right: 30px;
      }
      div:nth-of-type(2){
        position: relative;
         .srch-inp{
          display: inline-block;
          width: 120px;
          padding: 5px;
          box-sizing: border-box;
          outline: none;
          border: none;
          border-radius: 2px;
          font-size: 12px;
        }
        .srch-icon{
          position: absolute;
          right: 10px;
          top: 50%;
          transform: translateY(-50%);
          color: #ccc;
        }
      }
     
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
  .outer{
    background: #eee;
    padding: 0 25px;
    overflow: hidden;
    .main{
      width: 67%;
      margin: 50px 5px;
    }
    .list{
      width: 30%;
      margin: 50px 10px;
    }
  }
</style>
