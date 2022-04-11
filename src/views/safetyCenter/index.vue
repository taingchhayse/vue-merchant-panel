<template>
  <div class="dashboard-container">
    <div class="box box-primary">
          <div class="box-body box-profile">
            <h3 class="profile-username text-center">商户信息</h3>
            <ul class="list-group list-group-unbordered">
              <li class="list-group-item">
                <b>商户名称</b> <b class="pull-right">test</b>
              </li>
              <li class="list-group-item">
                <b>登录名</b> <b class="pull-right">test</b>
              </li>
              <li class="list-group-item">
                <b>入驻时间</b> <b class="pull-right">2022-04-09</b>
              </li>
              <li class="list-group-item">
                <b>谷歌验证器(Google Authenticator)</b> 
              </li>
              <li class="list-group-item">
                <b>登录IP白名单</b> 
              </li>


              <li class="list-group-item">

              </li>
            </ul>
          </div>
    </div>
    <div class="box box-primary">
          <div class="box-body box-profile">
            <h3 class="profile-username text-center">API 接口</h3>
            <ul class="list-group list-group-unbordered">
              <li class="list-group-item">
                <b>API MerchantId</b> <b class="pull-right">79759</b>
              </li>
              <li class="list-group-item">
                <b>API Md5Key</b> <b class="pull-right">****b92DL</b>
              </li>
              <li class="list-group-item">
                <b>API 调用IP白名单</b> <b class="pull-right">未绑定，请联系客服绑定，否则无法使用</b>
              </li>
              <li class="list-group-item">
                <b>API 接口文档</b> <b class="pull-right">请联系客服</b>
              </li>
            </ul>

          </div>
    </div>
    <div class="box box-primary">
          <div class="box-header with-border">
            <h3 class="box-title">登录记录</h3>
          </div>
          <div class="box-body">
              <strong><i class="fa fa-map-marker margin-r-5"></i> </strong><span class="text-muted">27.96.***.50</span>
              <p>2022-04-11 19:34:15</p>
              <strong><i class="fa fa-map-marker margin-r-5"></i> </strong><span class="text-muted">27.96.***.50</span>
              <p>2022-04-11 18:38:11</p>
              <strong><i class="fa fa-map-marker margin-r-5"></i> </strong><span class="text-muted">27.96.***.50</span>
              <p>2022-04-11 18:33:28</p>
              <strong><i class="fa fa-map-marker margin-r-5"></i> </strong><span class="text-muted">27.96.***.50</span>
              <p>2022-04-11 17:05:18</p>
              <strong><i class="fa fa-map-marker margin-r-5"></i> </strong><span class="text-muted">27.96.***.50</span>
              <p>2022-04-11 12:00:05</p>
              <strong><i class="fa fa-map-marker margin-r-5"></i> </strong><span class="text-muted">27.96.***.50</span>
              <p>2022-04-11 11:25:29</p>
              <strong><i class="fa fa-map-marker margin-r-5"></i> </strong><span class="text-muted">182.16.***.23</span>
              <p>2022-04-11 09:33:27</p>
              <strong><i class="fa fa-map-marker margin-r-5"></i> </strong><span class="text-muted">182.16.***.23</span>
              <p>2022-04-10 03:16:02</p>
              <strong><i class="fa fa-map-marker margin-r-5"></i> </strong><span class="text-muted">182.16.***.23</span>
              <p>2022-04-10 01:24:36</p>
              <strong><i class="fa fa-map-marker margin-r-5"></i> </strong><span class="text-muted">27.96.***.50</span>
              <p>2022-04-09 21:13:01</p>

          </div>
        </div>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  name: 'SafetyCenter',
  computed: {
    ...mapGetters([
      'name'
    ])
  }
}
</script>

<style lang="scss" scoped>
.text-cent{
  text-align: center;
}
.dashboard {
  &-container {
    margin: 30px;
  }
  &-text {
    font-size: 30px;
    line-height: 46px;
  }
  display: flex;
}
.box {
  display: block;
    position: relative;
    border-radius: 3px;
    background: #ffffff;
    border-top: 3px solid #d2d6de;
    margin-bottom: 20px;
    width: 50%;
    box-shadow: 0 1px 1px rgb(0 0 0 / 10%);
}
.box.box-primary {
    border-top-color: #3c8dbc;
}

</style>
