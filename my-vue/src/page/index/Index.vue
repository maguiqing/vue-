<template>
  <div >
     <header class="header">
       <div class="back">返回</div>
       <div class="search"></div>
       <div class="city">城市</div>
     </header>
     <swiper :options="swiperOption"  >
      <!-- slides -->
      <swiper-slide>
        <div class="swiper-img-con">
          <img class="swiper-img" src="//gw.alicdn.com/tfs/TB1hLaThf1TBuNjy0FjXXajyXXa-1125-352.jpg_760x760q75.jpg_.webp">
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="swiper-img-con">
         <img class="swiper-img"  src="//gw.alicdn.com/tfs/TB1hMHcg1SSBuNjy0FlXXbBpVXa-1125-352.jpg_760x760q75.jpg_.webp">
        </div>
      </swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
     </swiper>
  </div>
</template>

<script>
export default {
  name: 'Index',
  data () {
    return {
       swiperOption: {
          autoplay:true,
          direction:'horizontal'
        }
    }
  }
}
</script>

<style scoped>
   .header{
    display: flex;
    height: .86rem;
    background: #05bad5;
    color: #fff;
   }
   .back{ 
    width: .64rem;
    line-height: .86rem;
   }
   .search{
    flex: 1;
    margin: .14rem .18rem;
    background: #fff;
    border-radius: .1rem;
   }
   .city{
    width: 1.14rem;
    line-height: .86rem;
    text-align: center;
   }
   .swiper-img-con{
     width: 100%;

   }
   .swiper-img{
    width: 100%;
   }
</style>