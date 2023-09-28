<template>
    <div class="home-wrapper">
      <!-- <div v-for="item in list" :key="item" class="home-item">{{ item }}</div> -->
        

      <el-col :xs="24" :sm="20" :md="18" :lg="18" :xl="13">
        
        <div style="display: flex;flex-direction: column">
            
            <div v-for="item in list" :key="item" class="home-item" 
            style="
            border-style:solid;
            border-width:1px;
            border-color:#e2e8f0;
            border-radius: 8px;

            /* background-color: #f6f6f7; */
            margin-bottom:15px;
            box-shadow: 0px 1px 12px #d6d6d6;
            ">
                <div style="margin:8px 5px 10px 8px;font-size:16px;font-weight:bold">常用标签</div>
                <div style="border-top-style:solid;border-width:1px;border-color:#e2e8f0;"></div>
                <div style="padding: 10px; display: flex;flex-wrap: wrap;">
                    <div v-for="item in list" :key="item" class="home-item">
                        <el-col :xs="24" :sm="20" :md="18" :lg="18" :xl="13">
                            <div 
                            style="
                                display: flex;
                                border-style:solid;
                                border-width:1px;
                                border-color:#e2e8f0;
                                height: 50px;
                                max-width: 500px;
                                ">
                                <div><img src="/top_left_logo.png" alt="" style="min-width: 40px;height: 40px;"></div>
                                <div style="margin-left: 6px;">
                                    <div>Jungle Scout</div>
                                    <div style="color: #a2a2a2;">快速找到潜力爆款产品，预估销量和竞争的趋势</div>
                                </div>
                            </div>
                        </el-col>
                    </div>


                </div>
            </div>
        </div>
    
    </el-col>

      
    </div>
  </template>
  
  <script lang="ts" setup>
  import { ref } from 'vue'
  const list = [1, 2, 3, 4, 5, 6, 7, 8, 9];
  const linkList = ref([
        {
        name:"Vue3",
        icon:"https://avatars.githubusercontent.com/u/6128107?s=200&v=4",
        link:"https://cn.vuejs.org/"
        },
   ])

    // 新窗口打开外部链接
    const openLink=(url:string)=>{
        window.open(url,"_blank")
    }

  </script>
  
  <style scoped>

  .home-wrapper {
    display: flex;
    justify-content: center;
    margin-top: 40px;
  }

  .home-item {
    vertical-align: middle;
    margin: 4px 4px 10px;
    padding: 4px 8px;
    font-weight: bolder;
    display: inline-block;
    cursor: pointer;
    border-radius: 2px;
    line-height: 13px;
    font-size: 13px;
    box-shadow: 0 1px 8px 0 rgba(0, 0, 0, 0.1);
    transition: all 0.5s;
  }
  </style>