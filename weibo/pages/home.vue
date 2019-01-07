<template>
  <section class="container">
    <div class="top">
      <p><img src="../static/weibo.png" alt=""></p>
      <div class="inp">
        <input type="text" placeholder="大家都在搜：#大江大河#">
        <img src="../static/sousuo.png" alt="">
      </div>
      <p>
        <img src="../static/xinfeng.png" alt="">
        <img src="../static/shuru.png" alt="">
      </p>
    </div>
    <div class="nav">
      <ul>
        <li>
          <nuxt-link to="/home/hot" />热门</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/fangle" />新鲜事</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/nearby" />附近</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/funny" />搞笑</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/emotion" />情感</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/star" />明星</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/society" />社会</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/numerical" />数码</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/sports" />体育</nuxt-link>
        </li>
        <li>
          <nuxt-link to="car" />汽车</nuxt-link>
        </li>
        <li>
          <nuxt-link to="movies" />电影</nuxt-link>
        </li>
        <li>
          <nuxt-link to="game" />游戏</nuxt-link>
        </li>

      </ul>
    </div>
    <div class="main">
        <nuxt/>
    </div>
  </section>
</template>

<script>
    import Logo from '~/components/Logo.vue'

    export default {
        components: {
            Logo
        }
    }
</script>

<style>
    * {
        margin: 0;
        padding: 0;
    }
    
    html,
    body {
        width: 100%;
        height: 100%;
    }
    
    ul,
    ol,
    li {
        list-style: none;
    }
    
    .container {
        width: 100%;
        height: 100%;
        display: flex;
        flex-direction: column;
    }
    
    .top {
        width: 100%;
        height: 50px;
        display: flex;
        padding: 0 15px;
        box-sizing: border-box;
    }
    
    .top p {
        height: 100%;
    }
    
    .top .inp {
        flex: 1;
        position: relative;
        padding: 8px 6px;
        box-sizing: border-box;
    }
    
    .top .inp input {
        width: 100%;
        height: 100%;
        padding-left: 26px;
        box-sizing: border-box;
        border-radius: 8px;
        border: none;
        background: #eee;
    }
    
    .top img {
        width: 26px;
        height: 26px;
        margin-top: 12px;
        vertical-align: middle;
    }
    
    .top .inp img {
        position: absolute;
        left: 10px;
        top: 3px;
        vertical-align: middle;
        width: 20px;
        height: 20px;
    }
    
    .nav {
        width: 100%;
        height: 50px;
        border-bottom: 1px solid #ccc;
        padding: 0 10px;
        box-sizing: border-box;
    }
    
    .nav ul {
        width: 100%;
        height: 100%;
        line-height: 50px;
        overflow-x: scroll;
        white-space: nowrap;
    }
    
    .nav li {
        display: inline-block;
        margin-right: 12px;
        color: #666;
    }
    
    .main {
        flex: 1;
    }
</style>