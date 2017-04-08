<template>
    <div>
        <m-header title="豆瓣app" :bg="true" fixed>
            <a href="javascript:;" slot="right">分享</a>
        </m-header>
        <div class="page-content">
            <m-swipe swipeid="swipe01" :autoplay="1000" paginationDirection="right">
            <div class="swiper-slide slide01" slot="swiper-con">slide 01</div>
            <div class="swiper-slide slide01" slot="swiper-con">slide 02</div>
            <div class="swiper-slide slide01" slot="swiper-con">slide 03</div>
            </m-swipe>
        </div>
        <m-cell title="提醒" icon>
        <img src="../../assets/images/ic_mine_notification.png" slot="icon">
        <a href="javascript:;" slot="cell-right"><img src="../../assets/images/ic_arrow_gray_small.png" alt=""></a>
      </m-cell>
      <m-cell title="设置">
        <a href="javascript:;" slot="cell-right"><img src="../../assets/images/ic_arrow_gray_small.png" alt=""></a>
      </m-cell>
      <m-cell-media author="作者：大象公会" column="来自栏目：广播精选" img="https://qnmob2.doubanio.com/img/files/file-1489047494.jpg">
         <span slot="title">个人意见：为什么中国没有鲍勃·迪伦这样的民谣歌手</span>
         <span slot="describe">我们这一代人的成长年代，真正的诗歌课从来都是缺席的。</span>
       </m-cell-media>
    </div>
</template>

<script>
    import mHeader from '../../components/header'
    import mSwipe from '../../components/swipe'
    export default {
        name: 'index',
        components: {
            mHeader,
            mSwipe
        }
    }
</script>


<style lang="less">
.is-fixed ~ .page-content{
padding-top:44px;
}
.slide01{
    background: #41b883;
    text-align: center;
    line-height: 200px;
    font-size: 30px;
    color: #fff;
}
.slide02{
    background: #364a60;
    text-align: center;
    line-height: 200px;
    font-size: 30px;
    color: #fff;
}
.slide03{
    background: #ea6f5a;
    text-align: center;
    line-height: 200px;
    font-size: 30px;
    color: #fff;
}
</style>