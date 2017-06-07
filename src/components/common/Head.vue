<template>
  <div class="header">
    <div class="logo">后台管理系统</div>
    <div class="user-info">
      <el-dropdown>
        <div class="el-dropdown-link">
          <span class="header-touxiang"><img src="/static/images/touxiang.jpg"/></span>
          <span class="header-name">韩墨菲</span>
        </div>
        <el-dropdown-menu slot="dropdown">
          <el-dropdown-item>修改资料</el-dropdown-item>
          <el-dropdown-item>退出登录</el-dropdown-item>
        </el-dropdown-menu>
      </el-dropdown>
    </div>
  </div>
</template>
<script>
  export default{
    name: '',
    data(){
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }

  }
</script>

<style lang="scss" scoped>
  .header {
    position: relative;
    box-sizing: border-box;
    width: 100%;
    height: 70px;
    font-size: 22px;
    line-height: 70px;
    color: #fff;
  }

  .header .logo {
    float: left;
    width: 250px;
    text-align: center;
  }

  .user-info {
    float: right;
    padding-right: 50px;
    font-size: 16px;
    color: #fff;
  }

  .el-dropdown-link {
    height: 70px;
  }

  .header-touxiang {
    margin-top: 10px;
    width: 50px;
    height: 50px;
    display: inline-block;
    overflow: hidden;
    border-radius: 100%;
    vertical-align: top;
    & img {
      width: 100%;
      height: 100%;
    }
  }

  .header-name {
    color: #fff;
    display: inline-block;
    height: 50px;
    line-height: 50px;
    margin-left: 10px;
  }

</style>
