<template>
  <form action="" class="form-horizontal" >
    <div >
      <label class="col-md-3 control-label" >单据编号: </label>
      <label class="col-md-3 control-label" >客户代码: </label>
      <label class="col-md-3 control-label" >销售订单号: </label>
      <label class="col-md-3 control-label" >客户订单号: </label>
      <label class="col-md-3 control-label" >客户物料号: </label>
      <label class="col-md-3 control-label" >订单类型: </label>
      <select class="form-control">
        <option value="0"></option>
      </select>
    </div>
    <div >
      <label class="col-md-3 control-label" >产品内控参数: </label>
      <label class="col-md-3 control-label" >产品要求代码: </label>
      <label class="col-md-3 control-label" >产品类型: </label>
      <label class="col-md-3 control-label" >型号: </label>
      <label class="col-md-3 control-label" >产品规格: </label>
      <label class="col-md-3 control-label" >是否特殊订单: </label>
    </div>
    <div >
      <label class="col-md-3 control-label" >配比号: </label>
      <label class="col-md-3 control-label" >单位克重(g/cm2): </label>
      <label class="col-md-3 control-label" >数量（卷）: </label>
      <label class="col-md-3 control-label" >原料重量/kg: </label>
      <label class="col-md-3 control-label" >压花类型: </label>
      <label class="col-md-3 control-label" >切边类型: </label>
    </div>
    <div >
      <label class="col-md-3 control-label" >宽幅: </label>
      <label class="col-md-3 control-label" >中心值: </label>
      <label class="col-md-3 control-label" >接头数: </label>
      <label class="col-md-3 control-label" >缺陷数: </label>
      <label class="col-md-3 control-label" >接头和缺陷总数: </label>
      <label class="col-md-3 control-label" >每个补充米数: </label>
    </div>
    <div >
      <label class="col-md-3 control-label" >接头缺陷标识: </label>
      <label class="col-md-3 control-label" >标签颜色: </label>
      <label class="col-md-3 control-label" >标签模板: </label>
      <label class="col-md-3 control-label" >标签显示克重: </label>
      <label class="col-md-3 control-label" >产区: </label>
      <label class="col-md-3 control-label" >出口: </label>
    </div>
    <div >
      <label class="col-md-3 control-label" >标签要求: </label>
    </div>
    <div >
      <label class="col-md-3 control-label" >收卷方向: </label>
      <label class="col-md-3 control-label" >打包方式: </label>
    </div>
    <div >
      <label class="col-md-3 control-label" >辅料: </label>
      <label class="col-md-3 control-label" >装车要求: </label>
    </div>
    <div >
      <label class="col-md-3 control-label" >单: </label>
      <label class="col-md-3 control-label" >托: </label>
    </div>
    <div >
      <label class="col-md-3 control-label" >销售备注: </label>
    </div>
    <div >
      <label class="col-md-3 control-label" >内控备注: </label>
    </div>
    <div >
      <label class="col-md-3 control-label" >审核意见: </label>
    </div>
    <div >
      <label class="col-md-3 control-label" >手册号: </label>
      <label class="col-md-3 control-label" >压花前规格: </label>
      <label class="col-md-3 control-label" >压花后规格: </label>
      <label class="col-md-3 control-label" >制单人: </label>
    </div>
    <div >
      <label class="col-md-3 control-label" >批次代码: </label>
      <label class="col-md-3 control-label" >批次流水号: </label>
      <label class="col-md-3 control-label" >交货基地: </label>
      <label class="col-md-3 control-label" >制单时间: </label>
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
</style>
