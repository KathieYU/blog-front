<template>
  <div class="list-outer">
     <div class="list-meta">
          <a href="#">{{this.tag}}</a>
      </div>
      <div class="list-main">
          <div class="list-title">
              <a>title</a>
          </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'List',
  props: {
    tag:{
      type:String,
      default:'2020'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.list-outer{
  margin-bottom: 50px;
}
.list-meta{
        text-transform: uppercase;
        letter-spacing: 2px;
        margin-bottom: 1em;
        margin-left: 5px;
        line-height: 1em;
        text-shadow: 0 1px #fff;
        font-weight: bold;
        a{
         color: #999;
         margin: 0 0 14px 2px;
        }
    }
.list-main{
  color: #777;
  text-shadow: 0 1px #fff;
  background: #ddd;
  -webkit-box-shadow: 0 -1px 4px #ccc inset;
  box-shadow: 0 -1px 4px #ccc inset;
  border: 1px solid #ccc;
  padding: 15px;
  border-radius: 3px;
  .list-title a{
    color: #258fb8;
  }
}

</style>
