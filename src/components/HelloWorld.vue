<template>
  <form action="" >
    <div class="div-out">
      <div class="div-bind">
        <label>&emsp;&emsp;单据编号: </label>
        <el-input v-model="danID" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >&emsp;&emsp;&emsp;客户代码: </label>
        <el-input v-model="custCode" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>销售订单号: </label>
        <el-input v-model="saleOrder" readonly="true"  class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >&emsp;客户订单号: </label>
        <el-input v-model="custOrder" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>&emsp;&emsp;客户物料号: </label>
        <el-input v-model="custMat" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >&emsp;&emsp;&emsp;&emsp;订单类型: </label>
        <el-input v-model="orderType" readonly="true" class="input-width-short" ></el-input>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind">
        <label>产品内控参数: </label>
        <el-input v-model="proPara" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >&emsp;产品要求代码: </label>
        <el-input v-model="proCode" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>&emsp;产品类型: </label>
        <el-input v-model="proType" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >&emsp;&emsp;&emsp;&emsp;型号: </label>
        <el-input v-model="mtype" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>&emsp;&emsp;&emsp;产品规格: </label>
        <el-input v-model="proStand" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind-6">
        <label class="lab2">&emsp; 是否特殊订单: </label>
        <el-checkbox v-model="isSpecial" disabled></el-checkbox>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind">
        <label>&emsp;&emsp;&emsp;配比号: </label>
        <el-input v-model="matchID" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >单位克重(g/cm2): </label>
        <el-input v-model="perWeight" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>数量（卷）: </label>
        <el-input v-model="quantity" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >&nbsp;&nbsp;原料重量/kg: </label>
        <el-input v-model="matWeight" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>&emsp;&emsp;&emsp;压花类型: </label>
        <el-input v-model="embossType" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >&emsp;&emsp;&emsp;&emsp;切边类型: </label>
        <el-input v-model="cutType" readonly="true" class="input-width-short" ></el-input>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind">
        <label>&emsp;&emsp;&emsp;&emsp;宽幅: </label>
        <el-input v-model="input" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >&emsp;&emsp;&emsp;&emsp;中心值: </label>
        <el-input v-model="centerValue" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>&emsp;&emsp;接头数: </label>
        <el-input v-model="jointNunber" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >&emsp;&emsp;&emsp;缺陷数: </label>
        <el-input v-model="defectNumber" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>接头和缺陷总数: </label>
        <el-input v-model="jdNumber" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >每个缺陷补充米数: </label>
        <el-input v-model="persupply" readonly="true" class="input-width-short" ></el-input>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind">
        <label>接头缺陷标识: </label>
        <el-input v-model="jointDef" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >&emsp;&emsp;&emsp;标签颜色: </label>
        <el-input v-model="tagColor" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>&emsp;标签模板: </label>
        <el-input v-model="tagModel" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label >标签显示克重: </label>
        <el-input v-model="tagShowWeight" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind">
        <label>&emsp;&emsp;&emsp;&emsp;&emsp;产区: </label>
        <el-input v-model="proArea" readonly="true" class="input-width-short" ></el-input>
      </div>
      <div class="div-bind-6">
        <label class="lab2">&emsp;&emsp;&emsp;&emsp;&emsp;出口: </label>
        <el-checkbox v-model="isExport" disabled></el-checkbox>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-large">
        <div >
          <div class="div-bind-2">
            <label >标签要求:</label>
          </div>
          <div class="div-bind-3">
            <el-input type="textarea" v-model="tagReq" :rows="2" readonly class="text-mar"></el-input>
          </div>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-4">
        <label class="lab">收卷方向: </label>
        <el-input v-model="wrapupDir" readonly="true" class="input-width-medium" ></el-input>
      </div>
      <div class="div-bind-4">
        <label class="lab">打包方式: </label>
        <el-input v-model="wrapupWay" readonly="true" class="input-width-medium" ></el-input>
      </div>

    </div>
    <div class="div-out">
      <div class="div-bind-4">
        <label class="lab">&emsp;&emsp;辅料: </label>
        <el-input v-model="subMaterial" readonly="true" class="input-width-medium" ></el-input>
      </div>
      <div class="div-bind-4">
        <label class="lab">装车要求: </label>
        <el-input v-model="loadReq" readonly="true" class="input-width-medium" ></el-input>
      </div>

    </div>
    <div class="div-out">
      <div class="div-bind-4">
        <label class="lab">&emsp;&emsp;&emsp;单: </label>
        <el-input v-model="dan" readonly="true" class="input-width-medium" ></el-input>
      </div>
      <div class="div-bind-4">
        <label class="lab">&emsp;&emsp;&emsp;托: </label>
        <el-input v-model="pallet" readonly="true" class="input-width-medium" ></el-input>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-large">
        <div >
          <div class="div-bind-2">
            <label >销售备注:</label>
          </div>
          <div class="div-bind-3">
            <el-input type="textarea" v-model="saleRemark" :rows="2" readonly class="text-mar"></el-input>
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
            <el-input type="textarea" v-model="conRemark" :rows="2" readonly class="text-mar"></el-input>
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
            <el-input type="textarea" v-model="checkSug" :rows="2" readonly class="text-mar"></el-input>
          </div>
        </div>
      </div>
    </div>
    <div class="div-out">
      <div class="div-bind-5">
        <label class="lab">&emsp;手册号: </label>
        <el-input v-model="manualID" readonly="true" class="input-width-quarter" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab">压花前规格: </label>
        <el-input v-model="bembossStand" readonly="true" class="input-width-quarter" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab">压花后规格: </label>
        <el-input v-model="aembossStand" readonly="true" class="input-width-quarter" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab">&emsp;制单人: </label>
        <el-input v-model="madeby" readonly="true" class="input-width-quarter" ></el-input>
      </div>

    </div>
    <div class="div-out">
      <div class="div-bind-5">
        <label class="lab">批次代码: </label>
        <el-input v-model="batchCode" readonly="true" class="input-width-quarter" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab">批次流水号: </label>
        <el-input v-model="batchSerial" readonly="true" class="input-width-quarter" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab">&emsp;交货基地: </label>
        <el-input v-model="delArea" readonly="true" class="input-width-quarter" ></el-input>
      </div>
      <div class="div-bind-5">
        <label class="lab">制单时间: </label>
        <el-input v-model="madeTime" readonly="true" class="input-width-quarter" ></el-input>
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
  width: 30%;
  height: 50%;
  margin-top: 5%;
}
.input-width-medium{
  width: 70%;
  height: 50px;
  margin-top: 1%;
  margin-left: 3%;
}
.input-width-quarter{
  width: 50%;
  height: 50%;
  margin-top: 1%;
  margin-left: 3%;
  margin-bottom: 1%;
}
.div-bind{
  width: 15%;
  border:1px solid #ccc;
  float: left;
  box-sizing: border-box;
  height: 60px;
}
.div-bind-2{
  margin-top: 1.5%;
  margin-bottom: 1.5%;
  margin-left: 6%;
  width: 3%;
  float: left;
}
.div-bind-3{
  width: 90%;
  float: left;
}
.div-bind-4{
  width: 45%;
  border:1px solid #ccc;
  float: left;
  box-sizing: border-box;
  text-align: left;
}
.div-bind-5{
  width: 22.5%;
  border:1px solid #ccc;
  float: left;
  box-sizing: border-box;
  text-align: left;
}
.div-bind-6{
  width: 15%;
  border:1px solid #ccc;
  float: left;
  box-sizing: border-box;
  height: 60px;
  text-align: left;
  line-height: 60px;
}
.div-bind-large{
  width: 90%;
  border:1px solid #ccc;
  float: left;
  box-sizing: border-box;
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
  margin-top: 1%;
}
.lab2{
  margin-left: 10%;
  padding-right: 10%;
}
label{
  font-size: 8px;
  font-weight: bold;
}
</style>
