<template>
  <div class="body">
    <header class="header">
      
    </header>

    <section class="section">
      <div class="search">
        <img src="../img/banner.jpg" alt="">
      </div>

      <div class='list'>
        <dl v-for="(i,key) in newlist" :key="key">
          {{i.sorts}}
        </dl>
        <dl>
          <dt></dt>
          <dd>美食</dd>
        </dl>
        <dl>
          <dt></dt>
          <dd>电影/演出</dd>
        </dl>
        <dl>
          <dt></dt>
          <dd>酒店住宿</dd>
        </dl>
        <dl>
          <dt></dt>
          <dd>休闲娱乐</dd>
        </dl>
        <dl>
          <dt></dt>
          <dd>外卖</dd>
        </dl>
        <dl>
          <dt></dt>
          <dd>机票/火车票</dd>
        </dl>
        <dl>
          <dt></dt>
          <dd>KTV</dd>
        </dl>
        <dl>
          <dt></dt>
          <dd>周边游</dd>
        </dl>
        <dl>
          <dt></dt>
          <dd>丽人/美发</dd>
        </dl>
        <dl>
          <dt>
            <span class="ellipse">热门</span>
          </dt>
          <dd>美团旅行</dd>
        </dl>
      </div>

      <div class="clear"></div>

      <div class='img_list'>
        <dl class="dl_img">
          <dt>
            <h3>教师节</h3>
            <p>5折吃美食</p>
          </dt>
          <dd>
            <div class="img">
              <img src="../img/img1.jpg" alt="">
            </div>
          </dd>
        </dl>
        <dl class="dl_img">
          <dt>
            <h3>教师节</h3>
            <p>5折吃美食</p>
          </dt>
          <dd>
            <div class="img">
              <img src="../img/img1.jpg" alt="">
            </div>
          </dd>
        </dl>
        <dl class="dl_img">
          <dt>
            <h3>教师节</h3>
            <p>5折吃美食</p>
          </dt>
          <dd>
            <div class="img">
              <img src="../img/img1.jpg" alt="">
            </div>
          </dd>
        </dl>
        <dl class="dl_img">
          <dt>
            <h3>教师节</h3>
            <p>5折吃美食</p>
          </dt>
          <dd>
            <div class="img">
              <img src="../img/img1.jpg" alt="">
            </div>
          </dd>
        </dl>
        <dl class="dl_img">
          <dt>
            <h3>教师节</h3>
            <p>5折吃美食</p>
          </dt>
          <dd>
            <div class="img">
              <img src="../img/img1.jpg" alt="">
            </div>
          </dd>
        </dl>

      </div>
    </section>
    <footer class="footer">
      <a href="#">
        <i class="iconfont icon-fangzi"></i>
        <span>首页</span>
      </a>
      <a href="#">
        <i class=""></i>
        <span>首页</span>
      </a>
      <a href="#">
        <i class=""></i>
        <span>首页</span>
      </a>
      <a href="#">
        <i class=""></i>
        <span>首页</span>
      </a>
      <a href="#">
        <i class=""></i>
        <span>首页</span>
      </a>
    </footer>
  </div>
</template>

<script>
  export default{
    data () {
      return {
        "newlist" : [
          {
            "sorts" : "首页"
          }
        ]
      }
    }
  }
</script>

<style scoped>
      .body{
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        display: flex;
        flex-direction: column;
      }
      .list{
        padding-left: .1rem;
        padding-right: .1rem;
        padding-top: .1rem;
        background: #fff;
        display: flex;
        flex-wrap: wrap;
      }
      .list dl{
        width: 20%;
        margin-top: .1rem;
      }
      .list dl dt{
        width: .45rem;
        height: .45rem;
        margin: 0 auto;
        background: red;
        border-radius: 100%;
        position: relative;
      }
      .list dl dt img{
        width: 100%;
      }
      .list dl dd{
        text-align: center;
        padding-top: 5px;
        font-family: "heitisc";
        /*transform:  scale(0.8);*/
        box-sizing: border-box;
        white-space:nowrap;
        text-overflow: ellipsis;
        oveflow:hidden;
      }
      .ellipse{
        width: .35rem;
        height: .2rem;
        line-height: .18rem;
        display: block;
        position: absolute;
        background: red;
        border: 2px solid #fff;
        border-radius: .2rem;
        top: -.1rem;
        right: -.1rem;
        text-align: center;
        color: white;
        transform: scale(0.9);
      }
      .search{
        width: 100%;
      }
      .search img{
        width: 100%;
        height: 100%;
      }
      .header{
        height: .4rem;
      }
      .footer{
        display: flex;
      }
      .footer a{
        flex: 1;
        text-align: center;
      }
      .section{
        flex:1;
        overflow-y:scroll; 
        background: #eee;
      }
      .footer{
        height: .44rem;
        background: lightblue;
      }
      a{
        color:#757575;
        text-decoration: none;
      }
      .img_list{
        display:flex;
        flex-wrap: wrap;
        text-align: center;
        background: #fff;
      }
      .dl_img{
        width: 25%;
      }
      .img{
        width: 80%;
        margin: 0 auto;
      }
      .img img{
        width: 100%;
      }
      .clear{
        clear:both;
      }
     
</style>
