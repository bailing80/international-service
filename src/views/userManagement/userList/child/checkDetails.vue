<!--  查看详情界面  -->
<template>
  <el-dialog
    title="查看详情"
    :visible.sync="dialogTableVisible"
    width="70%"
    @close="dialogClose"
    :modal-append-to-body="false"
  >
    <el-form status-icon label-width="300px" class="el-form">
      <el-form-item label="用户名：" prop="companyAffiliation">
        <el-input type="text" style="width:165px" v-model="form.productName" :disabled="true"></el-input>
      </el-form-item>

      <el-form-item label="手机号：" prop="productLine">
        <el-input type="text" style="width:165px" v-model="form.productName" :disabled="true"></el-input>
      </el-form-item>

      <el-form-item label="邮箱：" prop="productModel" class="left:300px;">
        <el-input type="text" style="width:165px" v-model="form.productName" :disabled="true"></el-input>
      </el-form-item>

      <el-form-item label="机器编号：" prop="productName">
        <el-input type="text" style="width:165px" v-model="form.productName" :disabled="true"></el-input>
      </el-form-item>

      <el-form-item label="医院：" prop="productName">
        <el-input type="text" style="width:165px" v-model="form.productName" :disabled="true"></el-input>
      </el-form-item>

      <el-form-item label="国家：" prop="productName">
        <el-input type="text" style="width:165px" v-model="form.productName" :disabled="true"></el-input>
      </el-form-item>

      <el-form-item label="所属公司：" prop="productName">
        <el-input type="text" style="width:165px" v-model="form.productName" :disabled="true"></el-input>
      </el-form-item>
      <el-form-item label="上次登录时间：" prop="productName">
        <el-input type="text" style="width:165px" v-model="form.productName" :disabled="true"></el-input>
      </el-form-item>
      <el-form-item label="注册时间：" prop="productName">
        <el-input type="text" style="width:165px" v-model="form.productName" :disabled="true"></el-input>
      </el-form-item>

      <el-form-item>
        <el-button type="primary" @click="dialogClose">返回</el-button>
      </el-form-item>
    </el-form>
  </el-dialog>
</template>
<script>
import HeaderNav from '@/components/headerNav'
export default {
    data() {
        return {
            form: {
                companyName: '',
                companyIntroduce: '',
                companyLogo: '',
                companyTheme: '',
                InstruceUse: '',
                other: '',
                url: '',
            },
            addVideo: [1],
            addPdf: [1],
            fileList: '',
            dialogImageUrl: '',
            dialogVisible: false,
            dialogTableVisible: true,
        }
    },
    components: {
        HeaderNav,
    },
    methods: {
        //关闭
        dialogClose() {
            this.$emit('dialogClose')
        },
    },
}
</script>
<style lang='less' scoped>
.el-form {
    padding: 0 0 0 20%;
}
.clolos1 {
    width: 13px;
    height: 30px;
    background: #29affb;
    line-height: 30px;
    padding: 0 10px;
    border-radius: 15px;
    color: #fff;
    position: absolute;
    margin-left: 65.35%;
    margin-top: 8.48%;
    z-index: 1;
}
.clolos2 {
    width: 13px;
    height: 30px;
    background: #29affb;
    line-height: 30px;
    padding: 0 10px;
    border-radius: 15px;
    color: #fff;
    position: absolute;
    margin-left: 65%;
    margin-top: 7%;
}
.clolos3 {
    width: 13px;
    height: 30px;
    background: red;
    line-height: 30px;
    padding: 0 10px;
    border-radius: 15px;
    color: #fff;
    position: absolute;
    margin-left: calc(100% + 40px);
    margin-top: 10%;
}
.add_pdf {
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.12), 0 0 6px rgba(0, 0, 0, 0.04);
    width: 80%;
    position: relative;
    margin-top: 3%;
}
.basicinformation {
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.12), 0 0 6px rgba(0, 0, 0, 0.04);
    width: 80%;
    position: relative;
}
</style>

