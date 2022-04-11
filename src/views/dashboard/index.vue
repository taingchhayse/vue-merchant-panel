<template>
  <div class="dashboard-container">
    <section class="content">
    <div class="callout callout-success">
      <p><i class="fa fa-bullhorn"></i> 欢迎使用，感谢您的支持，祝您生活愉快！</p>
    </div>
    <h3>CNY</h3>
    <div class="row">
      <div class="col-md-3 col-sm-6 col-xs-12">
        <div class="info-box bg-aqua">
          <span class="info-box-icon"><i class="fa fa-cny"></i></span>
          <div class="info-box-content">
            <span class="info-box-text">今日充值</span>
            <span class="info-box-number"><small>¥</small> <span id="TodayPayOrderAmount"></span></span>
          </div>
        </div>
      </div>
      <div class="col-md-3 col-sm-6 col-xs-12">
        <div class="info-box bg-red">
          <span class="info-box-icon"><i class="icon ion-card"></i></span>
          <div class="info-box-content">
            <span class="info-box-text">今日提现</span>
            <span class="info-box-number"><small>¥</small> <span id="TodayWithdrawAmount"></span></span>
          </div>
        </div>
      </div>
      <div class="clearfix visible-sm-block"></div>
      <div class="col-md-3 col-sm-6 col-xs-12">
        <div class="info-box">
          <span class="info-box-icon bg-yellow"><i class="fa fa-history"></i></span>
          <div class="info-box-content">
            <span class="info-box-text">当前余额</span>
            <span class="info-box-number"><small>¥</small> <span id="BalanceAmount"></span></span>
          </div>
        </div>
      </div>
      <div class="col-md-3 col-sm-6 col-xs-12 hide" id="domFreezingAmount">
        <div class="info-box">
          <span class="info-box-icon bg-red"><i class="fa fa-history"></i></span>
          <div class="info-box-content">
            <span class="info-box-text">冻结中</span>
            <span class="info-box-number"><small>¥</small> <span id="FreezingAmount"></span></span>
          </div>
        </div>
      </div>
    </div>
    <div class="box">
      <div class="box-header with-border">
        <h3 class="box-title">服务</h3>
      </div>
      <div class="box-body">
        <div class="row">
          <div class="col-md-3 col-sm-6 col-xs-12">
            <div class="info-box bg-teal">
              <span class="info-box-icon"><i class="fa fa-skype"></i></span>

              <div class="info-box-content">
                <span class="info-box-text">Skype 客服</span>
                <span class="info-box-number" style="font-size: 20px; cursor: pointer;"><span id="a1" onclick="this.innerText='live:.cid.739b73df6668b283'">点击获取</span></span>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12">
            <div class="info-box bg-teal">
              <span class="info-box-icon"><i class="fa fa-send-o"></i></span>

              <div class="info-box-content">
                <span class="info-box-text">Telegram 客服</span>
                <span class="info-box-number" style="font-size: 20px; cursor: pointer;"><span id="a2" onclick="this.innerText='zxf_001'">点击获取</span></span>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12">
            <div class="info-box bg-teal">
              <span class="info-box-icon"><i class="fa fa-whatsapp"></i></span>

              <div class="info-box-content">
                <span class="info-box-text">WhatsApp 客服</span>
                <span class="info-box-number" style="font-size: 20px; cursor: pointer;"><span id="a3" onclick="this.innerText='+639693593333'">点击获取</span></span>
              </div>
            </div>
          </div>
          <div class="clearfix visible-sm-block"></div>
        </div>
      </div>
      <div class="box-footer">

      </div>
    </div>
    <div class="box">
      <div class="box-header with-border">
        <h3 class="box-title">小提示</h3>
      </div>
      <div class="box-body">
        <div class="row">
          <div class="col-xs-12">
            <ul>
              <li>我司支持禁用商户后台提现功能（即设定为只允许通过API提现），如有需要请联系客服为您配置。</li>
              <li>强烈建议您绑定谷歌身份验证器（菜单 - 安全中心 - 谷歌验证器）以增强安全性能。绑定后敏感操作都需填写验证码，验证码每30秒自动刷新，每个验证码仅生效一次。</li>
              <li>部分浏览器或操作系统存在兼容问题，造成页面样式错乱、日期选择插件无法弹出等显示问题，建议您按照以下顺序排除：<br>1、清除浏览器缓存。<br>2、使用最新版本的谷歌浏览器。<br>3、不要使用“隐私模式、无痕模式”等。<br>4、更换纯净的操作系统。<br>若问题依然存在，请联系客服。日期选择插件也可以手动输入，格式例如：1999-01-02 03:04:05</li>
              <li>浏览器的密码自动保存、自动填充功能可能会将密码自动填写到错误的位置，导致频繁密码错误。若频繁提示密码错误，请禁用自动填充功能，手动输入密码。</li>
            </ul>
          </div>
          <div class="clearfix visible-sm-block"></div>
        </div>
      </div>
      <div class="box-footer">
      </div>
    </div>
  </section>
  </div>
</template>

<script>
import { mapGetters } from "vuex";
import callout from "@/components/callout/index.vue";
export default {
  name: 'Dashboard',
  computed: {
    ...mapGetters(["name"]),
  },
  data() {
    return {
      balaneData: {
        icon: '12313',
        text: 'asdfadf'
      }
    }
  }
  // components: {
  //   'call-out' : callout
  // },
};
</script>

<style lang="scss" scoped>
.dashboard {
  &-container {
    margin: 30px;
  }
  &-text {
    font-size: 30px;
    line-height: 46px;
  }
}
</style>
