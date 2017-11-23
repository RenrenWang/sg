<template>
  <div class="product">
      <div class="tab">
          <ul class="tab-controller">
              <li @click="selectTab(index)"  :class="[{'active':v.isActive}]" v-for="(v,index) in tabs">{{v.name}}</li>
          </ul>
          <div class="tab-content">
                <tabContent1 v-show="tabs[0].isActive"/>
                <tabContent2 v-show="tabs[1].isActive"/>
          </div>
      </div>
       
  </div>
</template>

<script>

import  tabContent1 from './tabContent1'
import  tabContent2 from './tabContent2'
export default {
  name: 'product',
  data () {
    return {
       tabs:[
         {name:'基础信息',isActive:true},
         {name:'溯源管理',isActive:false},
         {name:'其他',isActive:false}

       ]
    }
  },
 methods:{
  selectTab(index){
    this.tabs.map((item,idnex)=>{
        item.isActive=false;
    });
    this.tabs[index].isActive=true; 
  }
 },
   components: {
  
    tabContent1,
    tabContent2
  }
}
</script>


<style scoped lang="scss">
@import "../../assets/style/base.scss";
.product{
    .tab{
     .tab-controller{
      height:rem(100px);
      position:fixed;
      top:0;
      width:100%;
       z-index:9999;
        display:flex;
        justify-content:center;
        align-items:center;
        background:#fff;
        li{
         flex:1;
         text-align:center;
          font-size:16px;
          color:#666;
          &.active{
            color:#55acef;
          }
        }
      }
      .tab-content{
        padding-top:rem(100px);
      }
    }
    
    
}

</style>