<template>
  <div>
    <div class="nav">
        <div class="text">执笔断月キ</div>
      <ul>
          <li>
            <img src="/static/img/vue_mh.png" class="images">
          </li>
          <li>12</li>
          <li>33</li>
          <li>44</li>
          <li>55</li>
      </ul>
    </div>
   <ul class="menu">
     <li class="atv">日常任务</li>
     <li>帮派成员</li>
     <li>打造记录</li>
   </ul>
    <!-- <div class="add"  @click=add()>添加时间</div>
        <div class="block"  v-for="(list,index) in inputList" :key="index">
          <span class="demonstration">默认</span>
          <el-date-picker 
            v-model="value1"
            type="datetime" :picker-options="pickerOptions"
            placeholder="选择日期时间">
          </el-date-picker>
        <div @click='del'>删除</div>
    </div> -->
    </div>
</template>


<script>
export default {
    data() {
      return {
        value1: '',
        value2: '',
        value3: '',
        inputList:[],
        model:[],
      };
    },
    methods:{   
      add(){
        // this.value1='2019-10-03 00:00:00'
         this.inputList.push({});
      },
      del(index){
        // alert(this.inputList.length)
        // this.inputList.splice(index,1);
        if(window.confirm('确认删除'+this.value1+'吗')){
          this.inputList.splice(index,1)
        }
      }
    }
  };
</script>
<style lang="less">
  
</style>