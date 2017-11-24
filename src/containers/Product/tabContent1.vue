<template>
  <div class="tabContentBase">
       
                     <carousel paginationActiveColor="#fff"  :paginationPadding=3  :paginationSize=6  paginationColor="#dbdbdb" :perPage=1>
           <slide>
            <img  src="https://imgjd2.fruitday.com/images/product_pic/3877/1/1-370x370-3877-BXDY6KCU.jpg"/>
            </slide>
            <slide>
             <img  src="https://imgjd2.fruitday.com/images/product_pic/424/1/1-370x370-424-C59THSTC.jpg"/>
           </slide>
    </carousel>
    <div class="top-text">
         <h2>欢乐时光水果礼篮欢乐时光水果礼篮欢乐时光水果礼篮欢乐时光水果礼篮</h2>

    </div>
    <div class="d-text">
         <div class="d-title">
             <h3>产品信息</h3>
          </div>   
          <ul class="d-list">
               <li>
                  <span class="name">批次号:</span>
                  <span class="value">2588741255</span>
               </li> 
                <li>
                  <span class="name">产品类别:</span>
                  <span class="value">类别1</span>
               </li> 
                <li>
                  <span class="name">生产区块:</span>
                  <span class="value">区块1</span>
               </li> 
                <li>
                  <span class="name">建档日期:</span>
                  <span class="value">2017-08-06</span>
               </li> 
                <li>
                  <span class="name">录入人员:</span>
                  <span class="value">人员1</span>
               </li> 
                 <li>
                  <span class="name">状态:</span>
                  <span class="value">状态1</span>
               </li> 
          </ul>
    </div>
        <div class="d-text">
            <div class="d-title">
                <h3>产品介绍</h3>
            </div>
            <ul class="img-list">
                <li><img  src="../../assets/images/1.gif"></li>
                <li><img  src="../../assets/images/2.gif"></li>
                <li><img  src="../../assets/images/3.gif"></li>
                    <li><img  src="../../assets/images/4.gif"></li>
            </ul>
        </div>
  </div>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel';
export default {
  name: 'tabContentBase',
  data () {
    return {
    
    }
  },
  components:{
    Carousel,
    Slide
  }
}
</script>

<style scoped lang="scss">
@import "../../assets/style/base.scss";
.tabContentBase{
.VueCarousel-slide{
        img{
        height:rem(480px);
        width:100%;
        }
        
    }
    .VueCarousel-pagination{

        position: absolute;
        bottom:rem(300px);
    
    }

    .top-text{
      background:#fff;
       min-height:rem(150px);
       padding:rem(15px) rem(20px);
     
       h2{
           line-height:25px;
           font-size:18px;
           color:#000;
       }
    }
    .d-text{
      margin-top:rem(20px);
      padding:0  rem(20px);
      background:#fff;  
      .d-title{
         padding:rem(20px) 0 rem(15px) 0;
         h3{
             font-size:18px;
             border-left:3px solid #55acef;
             padding-left:10px;
             color:#8d969b;
         }
      }
      .d-list{
        display:flex;
        flex-wrap:wrap;

        li{
          width:50%;
          margin:rem(20px) 0;
          font-size:16px;
          .name{
             color:#8d969b;
          }
          .value{
            color:#000;
          }
        }
      }
      .img-list{
        margin-top:rem(20px);
        img{
          width:100%;
        }
      }

    }
        
}
 
</style>
