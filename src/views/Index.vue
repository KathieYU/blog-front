<template>
    <div>
        <div class="article-meta">
            <a href="#">2020-2-16</a>
        </div>
        <div class="article-main">
            <div class="article-title">
                title
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss">
    .article-meta{
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
    .article-main{
        background: #fff;
        box-shadow: 1px 2px 3px #ddd;
        border: 1px solid #ddd;
        border-radius: 3px;
    }
</style>