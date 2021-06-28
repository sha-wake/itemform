<template>
  <form action="" >
    <div class="div-out">
      <div class="div-bind">
          <div class="div-bind-10">
            <label >单据编号:</label>
          </div >
          <div class="div-bind-8">
            <el-input v-model="custCode" readonly="true" class="input-width-short" size="small"></el-input>
          </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >客户代码:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="custCode" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-7">
          <label >&emsp;&emsp;销售&ensp;<br>&emsp;订单号:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="saleOrder" readonly="true"  class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-7">
          <label >&emsp;&emsp;客户&ensp;<br>&emsp;订单号:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="custOrder" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-7">
          <label >&emsp;&emsp;客户&ensp;<br>&emsp;物料号:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="custMat" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >订单类型:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="orderType" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind">
        <div class="div-bind-7">
          <label >&emsp;产品内&ensp;<br>&emsp;控参数:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="proPara" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-7">
          <label >&emsp;产品要&ensp;<br>&emsp;求代码:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="proCode" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >产品类型:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="proType" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >&emsp;&emsp;型号:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="mtype" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >&emsp;&emsp;产品:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="proStand" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind-6">
        <div class="div-bind-7">
          <label >&emsp;是否特&ensp;<br>&emsp;殊订单:</label>
        </div >
        <div class="div-bind-9">
          <el-checkbox v-model="isSpecial"  disabled></el-checkbox>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind">
        <div class="div-bind-10">
          <label >&emsp;配比号:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="matchID" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-7">
          <label >单位克重<br>&ensp;(g/cm2):</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="perWeight" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >&ensp;数量(卷):</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="quantity" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-7">
          <label >原料重量<br>&emsp;&emsp;(/kg):</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="matWeight" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >压花类型:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="embossType" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >切边类型:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="cutType" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind">
        <div class="div-bind-10">
          <label >&emsp;&emsp;宽幅:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="input" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >&emsp;中心值:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="centerValue" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >&emsp;接头数:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="jointNunber" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >&emsp;缺陷数:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="defectNumber" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-7">
          <label >&ensp;接头和<br>缺陷总数:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="jdNumber" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-7">
          <label >每个缺陷<br>补充米数:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="persupply" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind">
        <div class="div-bind-7">
          <label >&emsp;接头缺<br>&emsp;陷标识:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="jointDef" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >标签颜色:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="tagColor" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >标签模板:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="tagModel" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-7">
          <label >&emsp;标签显<br>&emsp;示克重:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="tagShowWeight" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind">
        <div class="div-bind-10">
          <label >&emsp;&emsp;产区:</label>
        </div >
        <div class="div-bind-8">
          <el-input v-model="proArea" readonly="true" class="input-width-short" size="small" ></el-input>
        </div>
      </div>
      <div class="div-bind-6">
        <div class="div-bind-10">
          <label >&emsp;&emsp;出口:</label>
        </div >
        <div class="div-bind-9">
          <el-checkbox v-model="isExport" disabled></el-checkbox>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-large">
        <div >
          <div class="div-bind-2">
            <label >标签要求:</label>
          </div>
          <div class="div-bind-3">
            <el-input type="textarea" v-model="tagReq" :rows="1" readonly class="text-mar"></el-input>
          </div>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-4">
        <label class="lab">收卷方向: </label>
        <el-input v-model="wrapupDir" readonly="true" class="input-width-medium" size="small"></el-input>
      </div>
      <div class="div-bind-4">
        <label class="lab">打包方式: </label>
        <el-input v-model="wrapupWay" readonly="true" class="input-width-medium" size="small"></el-input>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-4">
        <label class="lab">&emsp;&emsp;辅料: </label>
        <el-input v-model="subMaterial" readonly="true" class="input-width-medium" size="small"></el-input>
      </div>
      <div class="div-bind-4">
        <label class="lab">装车要求: </label>
        <el-input v-model="loadReq" readonly="true" class="input-width-medium" size="small"></el-input>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-4">
        <label class="lab">&emsp;&emsp;&emsp;单: </label>
        <el-input v-model="dan" readonly="true" class="input-width-medium" size="small"></el-input>
      </div>
      <div class="div-bind-4">
        <label class="lab">&emsp;&emsp;&emsp;托: </label>
        <el-input v-model="pallet" readonly="true" class="input-width-medium" size="small"></el-input>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-large">
        <div >
          <div class="div-bind-2">
            <label >销售备注:</label>
          </div>
          <div class="div-bind-3">
            <el-input type="textarea" v-model="saleRemark" :rows="1" readonly class="text-mar"></el-input>
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
            <el-input type="textarea" v-model="conRemark" :rows="1" readonly class="text-mar"></el-input>
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
            <el-input type="textarea" v-model="checkSug" :rows="1" readonly class="text-mar"></el-input>
          </div>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-5">
        <label class="lab2">&emsp;手册号: </label>
        <el-input v-model="manualID" readonly="true" class="input-width-quarter" size="small" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab2">压花前规格: </label>
        <el-input v-model="bembossStand" readonly="true" class="input-width-quarter" size="small" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab2">压花后规格: </label>
        <el-input v-model="aembossStand" readonly="true" class="input-width-quarter" size="small" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab2">&emsp;制单人: </label>
        <el-input v-model="madeby" readonly="true" class="input-width-quarter" size="small" ></el-input>
      </div>

    </div>
    <div class="div-out">
      <div class="div-bind-5">
        <label class="lab2">批次代码: </label>
        <el-input v-model="batchCode" readonly="true" class="input-width-quarter" size="small" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab2">批次流水号: </label>
        <el-input v-model="batchSerial" readonly="true" class="input-width-quarter" size="small" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab2">&emsp;交货基地: </label>
        <el-input v-model="delArea" readonly="true" class="input-width-quarter" size="small" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab2">制单时间: </label>
        <el-input v-model="madeTime" readonly="true" class="input-width-quarter" size="small" ></el-input>
      </div>
    </div>
  </form>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
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
  width: 100%;
  height: 50%;
  margin-bottom: 5%;
}
.input-width-medium{
  width: 70%;
  height: 50px;
  margin-top: 1.5%;
  margin-left: 3%;
}
.input-width-quarter{
  width: 50%;
  height: 50%;
  margin-top: 3%;
  margin-left: 5%;
  margin-bottom: 1%;
}
.div-bind{
  width: 15%;
  border:1px solid #c6e2ff;
  float: left;
  box-sizing: border-box;
  height: 50px;
  background: #F8F9F9;
}
.div-bind-2{
  margin-top: 1.7%;
  margin-bottom: 1.5%;
  margin-left: 5%;
  width: 10%;
  float: left;
}
.div-bind-3{
  width: 80%;
  float: left;
  height: 30%;
}
.div-bind-4{
  width: 45%;
  border:1px solid #c6e2ff;
  float: left;
  box-sizing: border-box;
  text-align: left;
  height: 50px;
  background: #F8F9F9;
}
.div-bind-5{
  width: 22.5%;
  border:1px solid #b3d8ff;
  float: left;
  box-sizing: border-box;
  text-align: left;
  background: #F8F9F9;
  height: 50px;
}
.div-bind-6{
  width: 15%;
  border:1px solid #c6e2ff;
  float: left;
  box-sizing: border-box;
  height: 50px;
  background: #F8F9F9;
}
.div-bind-7{
  width: 45%;
  float: left;
  margin-top: 3%;
}
.div-bind-8{
  width: 50%;
  float: left;
  margin-top: 5%;
}
.div-bind-9{
  width: 30%;
  float: left;
  margin-top: 8%;
  margin-left: 10%;
}
.div-bind-10{
  width: 45%;
  float: left;
  margin-top: 8%;
}
.div-bind-large{
  width: 90%;
  border:1px solid #c6e2ff;
  float: left;
  box-sizing: border-box;
  background: #F8F9F9;
}
.div-out{
  margin-left: 20%;
  margin-right: 20%;
}
.text-mar{
  margin-bottom: 10px;
  margin-top: 10px;
  width: 90%;
  margin-left: 1%;
}
.lab{
  margin-left: 7%;
  margin-top: 3%;
}
.lab2{
  margin-left: 10%;
  margin-top: 1%;
}
label{
  font-size: 8px;
  font-weight: bold;
  color: #53a8ff;
  /*color: #2D2D2D;*/
}
</style>
