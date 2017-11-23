<template>
  <div class="tabContentitem">
       <div class="d-text" v-for="(v,index)">
         <div class="d-title">
              <h3>产品种源信息</h3>
          </div>   
          <ul class="d-list">
               <li>
                  <span class="name">批次号:</span>
                  <span class="value">2588741255</span>
               </li> 
           
          </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'tabContentitem',
  data () {
    return {
       data:[
           {name:"产品种源信息",list:[
               {name:'品种源编号',value:'12554'},
               {name:'种子名称',value:'12554'},
               {name:'种子来源',value:'12554'},
               {name:'种子状态',value:'12554'},
                {name:'育种方式',value:'12554'},
                {name:'是否是基因工程',value:'12554'},
                {name:'是否进过化学及辐射处理',value:'12554'},
                {name:'厂商名称',value:'12554'},
                {name:'地址',value:'12554'},
                 {name:'联系方式',value:'12554'},
                  {name:'种源购买日期',value:'12554'},
                   {name:'备注',value:'备注'}
                
           ]}
       ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../../assets/style/base.scss";
.tabContentitem{
     .d-text{
      margin-top:rem(20px);
      padding:0  rem(20px);
      background:#fff;  
      .d-title{
         padding:rem(15px) 0;
         h3{
             font-size:16px;
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
          margin:rem(30px) 0;
          font-size:16px;
          .name{
             color:#8d969b;
          }
          .value{
            color:#000;
          }
        }
      }
     }
}
  
</style>