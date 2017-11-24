<template>
  <div class="tabContentitem">
       <div class="d-text" v-for="(v,index) in data">
         <div class="d-title">
              <h3>{{v.name}}</h3>
          </div>   
          <ul class="d-list">
               <li v-for="(sv,sinde) in v.list">
                  <span class="name">{{sv.name}}:</span>
                  <span class="value">{{sv.value}}</span>
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
                
           ]},
            {name:"病虫草害防治信息",list:[
               {name:'病虫草害名称',value:'12554'},
               {name:'发生时间',value:'12554'},
               {name:'防治方式',value:'12554'},
               {name:'防治措施',value:'12554'},
                {name:'是否使用化学产品',value:'12554'},
                {name:'备注',value:'12554'},
         ]},
            {name:"产品防疫情况",list:[
               {name:'每次剂量',value:'12554'},
               {name:'防疫日期',value:'12554'},
               {name:'负责人',value:'12554'},
               {name:'防疫效果',value:'12554'},
                {name:'备注',value:'12554'}
            
                
           ]}, {name:"产品施肥情况",list:[
               {name:'化肥种类',value:'12554'},
               {name:'施肥时间',value:'12554'},
               {name:'施肥作物',value:'12554'},
               {name:'施肥量',value:'12554'},
                {name:'施肥人',value:'12554'},
                {name:'备注',value:'12554'}
            
           
           ]},
            {name:"产品收获信息",list:[
               {name:'收获时间',value:'12554'},
               {name:'收获方式',value:'12554'},
               {name:'收获总量',value:'12554'},
               {name:'收获批次设置',value:'12554'},
                {name:'优选等级',value:'12554'},
                {name:'备注',value:'12554'}
                
                
           ]},
            {name:"产品检测信息",list:[
               {name:'检测日期',value:'12554'},
               {name:'检测方式',value:'12554'},
               {name:'检测项目',value:'12554'},
               {name:'测试结果',value:'12554'}
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