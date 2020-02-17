<template>
  <div class="archives">  
    <div class="archives-meta">
        <a href="#">2020</a>
    </div>
    <div class="archives-main">
        <div class="archives-date">
          <a href="#">date</a>
        </div>
        <div class="archives-title">
          <a href="#">title</a>
        </div>
    </div>
  </div>
</template>
<script>
export default {
  
}
</script>
<style lang="scss">
.archives{
  width: 35%;
}
.archives-meta{
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
.archives-main{
  padding: 10px;
  margin-bottom: 30px;
  background: #fff;
  box-shadow: 1px 2px 3px #ddd;
  border: 1px solid #ddd;
  border-radius: 3px;
  .archives-date a{
    font-size: 12px;
    color: #999;
    margin-bottom: 8px;
  }
  .archives-title a{
    font-weight: bold;
    color: #555;
    font-size: 18px;
    &:hover{
      color: #258fb8;
    }
  }
}
</style>
