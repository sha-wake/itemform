<template>
  <form action="" class="form-horizontal" >
    <div class="div-out">
      <div class="div-bind">
        <label>单据编号: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >客户代码: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>销售订单号: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >客户订单号: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>客户物料号: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >订单类型: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind">
        <label>产品内控参数: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >产品要求代码: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>产品类型: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >型号: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>产品规格: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >是否特殊订单: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind">
        <label>配比号: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >单位克重(g/cm2): </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>数量（卷）: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >原料重量/kg: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>压花类型: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >切边类型: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind">
        <label>宽幅: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >中心值: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>接头数: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >缺陷数: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>接头和缺陷总数: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >每个补充米数: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind">
        <label>接头缺陷标识: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >标签颜色: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>标签模板: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >标签显示克重: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>产区: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >出口: </label>
        <el-input v-model="input" :disabled="true" class="input-width-short" ></el-input>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-large">
        <div >
          <div class="div-bind-2">
            <label >标签要求:</label>
          </div>
          <div class="div-bind-3">
            <el-input type="textarea" v-model="tag_requirement" :rows="2" disabled class="text-mar"></el-input>
          </div>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-4">
        <label class="lab">收卷方向: </label>
        <el-input v-model="input" :disabled="true" class="input-width-medium" ></el-input>
      </div>
      <div class="div-bind-4">
        <label class="lab">打包方式: </label>
        <el-input v-model="input" :disabled="true" class="input-width-medium" ></el-input>
      </div>

    </div>
    <div class="div-out">
      <div class="div-bind-4">
        <label class="lab">辅料: </label>
        <el-input v-model="input" :disabled="true" class="input-width-medium" ></el-input>
      </div>
      <div class="div-bind-4">
        <label class="lab">装车要求: </label>
        <el-input v-model="input" :disabled="true" class="input-width-medium" ></el-input>
      </div>

    </div>
    <div class="div-out">
      <div class="div-bind-4">
        <label class="lab">单: </label>
        <el-input v-model="input" :disabled="true" class="input-width-medium" ></el-input>
      </div>
      <div class="div-bind-4">
        <label class="lab">托: </label>
        <el-input v-model="input" :disabled="true" class="input-width-medium" ></el-input>
      </div>

    </div>
    <div class="div-out">
      <div class="div-bind-large">
        <div >
          <div class="div-bind-2">
            <label >销售备注:</label>
          </div>
          <div class="div-bind-3">
            <el-input type="textarea" v-model="tag_requirement" :rows="2" disabled class="text-mar"></el-input>
          </div>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-large">
        <div >
          <div class="div-bind-2">
            <label >内控备注:</label>
          </div>
          <div class="div-bind-3">
            <el-input type="textarea" v-model="tag_requirement" :rows="2" disabled class="text-mar"></el-input>
          </div>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-large">
        <div >
          <div class="div-bind-2">
            <label >审核意见:</label>
          </div>
          <div class="div-bind-3">
            <el-input type="textarea" v-model="tag_requirement" :rows="2" disabled class="text-mar"></el-input>
          </div>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-5">
        <label class="lab">手册号: </label>
        <el-input v-model="input" :disabled="true" class="input-width-quarter" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab">压花前规格: </label>
        <el-input v-model="input" :disabled="true" class="input-width-quarter" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab">压花后规格: </label>
        <el-input v-model="input" :disabled="true" class="input-width-quarter" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab">制单人: </label>
        <el-input v-model="input" :disabled="true" class="input-width-quarter" ></el-input>
      </div>

    </div>
    <div class="div-out">
      <div class="div-bind-5">
        <label class="lab">批次代码: </label>
        <el-input v-model="input" :disabled="true" class="input-width-quarter" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab">批次流水号: </label>
        <el-input v-model="input" :disabled="true" class="input-width-quarter" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab">交货基地: </label>
        <el-input v-model="input" :disabled="true" class="input-width-quarter" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab">制单时间: </label>
        <el-input v-model="input" :disabled="true" class="input-width-quarter" ></el-input>
      </div>

    </div>
  </form>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.input-width-short{
  width: 50%;
  height: 50px;
  margin-top: 3%;
  margin-left: 2px;
}
.input-width-medium{
  width: 80%;
  height: 50px;
  margin-top: 1%;
  margin-right: 1%;
}
.input-width-quarter{
  width: 75%;
  height: 50px;
  margin-top: 3%;
  margin-right: 1%;
}
.div-bind{
  width: 16%;
  border:1px solid #ccc;
  float: left;
  box-sizing: border-box;
}
.div-bind-2{
  margin-top: 1%;
  margin-bottom: 1%;
  margin-left: 5%;
  width: 5%;
  float: left;
}
.div-bind-3{
  width: 90%;
  float: left;
}
.div-bind-4{
  width: 48%;
  border:1px solid #ccc;
  float: left;
  box-sizing: border-box;
  text-align: left;
}
.div-bind-5{
  width: 24%;
  border:1px solid #ccc;
  float: left;
  box-sizing: border-box;
  text-align: left;
}
.div-bind-large{
  width: 96%;
  border:1px solid #ccc;
  float: left;
  box-sizing: border-box;
}
.div-out{
  margin-left: 3%;
}
.text-mar{
  margin-bottom: 10px;
  margin-top: 10px;
  width: 90%;
  margin-left: 1%;
}
.lab{
  margin-left: 5%;
  margin-top: 1%;
}

</style>
