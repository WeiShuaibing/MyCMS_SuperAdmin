<template>
  <div class="main">
    <div>
      <h2>添加站点：</h2>
    </div>
    <el-row :gutter="100">
      <el-col :span="6">
        <MDinput :maxlength="100" name="name" required>
          网站唯一标识：
        </MDinput>
      </el-col>
      <el-col :span="6">
        <MDinput :maxlength="100" name="name" required>
          网站名称：
        </MDinput>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="24">
        <MDinput :maxlength="100" name="name" required>
          域名URL：
        </MDinput>
        <!--<el-input placeholder="请输入内容">-->
        <!--<template slot="prepend">Http://</template>-->
        <!--</el-input>-->
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="24">
        <div class="beizhu">
          备注信息：
        </div>
        <el-input
          :rows="4"
          type="textarea"
          placeholder="备注信息..."
        />
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="24">
        <div class="commit">
          <el-button type="primary" size="medium">&nbsp;&nbsp;添&nbsp;加&nbsp;&nbsp;</el-button>
        </div>
      </el-col>
    </el-row>

  </div>
</template>

<script>
import MDinput from '@/components/MDinput'
export default {
  name: 'Addweb',
  components: { MDinput },
  data() {
    return {

    }
  }
}
</script>

<style scoped>
.main{
  width: 100%;
  height: 600px;
  padding: 32px;
  padding-left: 50px;
}
.el{
  width: 50%;
  display: inline;
}
.beizhu{
  color: #9E9E9E;
  font-size: 18px;
  height: 70px;
  line-height: 70px;
  font-family: Helvetica Neue, Helvetica, PingFang SC, Hiragino Sans GB, Microsoft YaHei, Arial, sans-serif;
}
.commit{
  margin-top: 60px;
  float: right;
}
</style>
