<template>
  <div>
    <div class="mu-banner">
      <div class="mu-banner-container">
        <div class="mu-logo">
          M
        </div>
        <h1 class="mu-banner-title">
          Muse-UI
        </h1>
        <h2 class="mu-banner-sub-title">
          基于 Vue 2.0 和 Material Desigin 开发的 UI 组件库
        </h2>
        <div class="mu-banner-actions">
          <mu-raised-button label="Get Started" color="lightBlue"/>
        </div>
      </div>
      <div class="mu-banner-appbar-height"></div>
    </div>
    <div class="mu-desc-wrapper">
      <div class="mu-desc">
        <h2 class="mu-desc-title">特性</h2>
        <mu-row gutter>
          <mu-col tablet="33" pc="33" class="mu-desc-item">
            <h3 class="mu-desc-sub-title">组件丰富</h3>
            <div class="mu-desc-text">
              Muse UI 基本实现了 Material Design 设计规范类的所有组件，
              另外还开发去多的功能性的组件
            </div>
          </mu-col>
          <mu-col tablet="33" pc="33" class="mu-desc-item">
            <h3 class="mu-desc-sub-title">可定制</h3>
            <div class="mu-desc-text">
              Muse UI 使用less文件，所有的颜色都有一个变量维护，通过编写 less 文件完成自定义主题，
              另外组件内部也提供一些修改效果的参数
            </div>
          </mu-col>
          <mu-col tablet="33" pc="33" class="mu-desc-item">
            <h3 class="mu-desc-sub-title">基于 Vue 2.0</h3>
            <div class="mu-desc-text">
              Muse UI 基于 Vue2.0 开发，Vue2.0是当下最快的前端框架之一，小巧，api友好，可用于开发的复杂单页应用
            </div>
          </mu-col>
        </mu-row>
      </div>
    </div>
    <div class="mu-footer">
      Muse-UI is open source and released under the MIT Licence.<br/>
      Copyright (c) 2016 myron
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style lang="less">
@import "../../src/styles/vars.less";
.mu-banner{
  background-color: @primary1Color;
  z-index: 100;
}

.mu-banner-appbar-height{
  height: 56px;
}

.mu-banner-container {
  margin-right: auto;
  margin-left: auto;
  padding-left: 24px;
  padding-right: 24px;
}

.mu-logo{
  width: 100px;
  height: 100px;
  line-height: 100px;
  text-align: center;
  background-color: @canvasColor;
  margin:  0 auto;
  color: @primary1Color;
  font-size: 50px;
  border-radius: 50%;
  margin-bottom: 16px;
}

.mu-banner-title{
  font-weight: 300;
  color: fade(@alternateTextColor, 87%);
  margin-top: 0;
  margin-bottom: 16px;
  text-align: center;
}

.mu-banner-sub-title{
  color: fade(@alternateTextColor, 87%);
  text-align: center;
  font-weight: 300;
  margin-bottom: 16px;
}

.mu-banner-actions{
  text-align: center;
}
.mu-desc-wrapper{
  background-color: @accent2Color;
}
.mu-desc{
  padding: 24px 24px 48px 24px;
  max-width: 800px;
  margin: auto;
}

.mu-desc-title{
  font-weight: 400;
  padding-left: 16px;
  padding-right: 16px;
}

.mu-desc-sub-title{
  font-weight: 400;
  font-size: 18px;
}

.mu-desc-item {
  padding-left: 16px;
  padding-right: 16px;
}
@media (min-width: 480px) {
  .mu-banner-appbar-height{
    height: 64px;
  }
}

.mu-footer{
  padding: 16px;
  background-color: @grey900;
  text-align: center;
  color: @white;
}
</style>
