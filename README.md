> 官网: [https://haomo-tech.com](https://haomo-tech.com)

> 作者: 毫末科技

> 邮箱: hxg@haomo-studio.com

## 预览

![预览图片](http://downloads.haomo-tech.com/uniapp/hm-balance-card.png)

[在线效果预览](http://template.uniapp.haomo-tech.com/pages/haomo/test-component/hm-balance-card)

更多毫末科技的uni-app跨端模板，请见[毫末科技uni-app跨端模板](https://haomo-tech.com/sale.html)

## 技术支持

* [uni-app插件市场](https://ext.dcloud.net.cn/plugin?id=1523)

* [npm包](https://www.npmjs.com/package/hm-uniapp-balance-card)

* [github地址](https://github.com/haomo-studio/hm-uniapp-balance-card)

* [gitee地址](https://gitee.com/haomo/hm-uniapp-balance-card)

毫末科技将长期迭代本组件。需要技术支持，请进钉钉群（群号30423559）：

<img width="250" src="http://downloads.haomo-tech.com/%E6%AF%AB%E6%9C%ABuniapp%E7%BB%84%E4%BB%B6%E6%8A%80%E6%9C%AF%E6%94%AF%E6%8C%81.jpg">

## 概述

毫末uni-app毫末余额卡片组件。支持H5/小程序(微信、支付宝、头条、百度、QQ)/App；组件可自适应各种屏幕大小的手机。

## 使用

请使用HBuilderX导入组件。

在script中引用：

```javascript
import HmBalanceCard from '@/components/hm-balance-card/index.vue'
export default {
    components: { HmBalanceCard }
}
```

在template中使用：

```html
<template>
  <div class="test-component">
    <hm-balance-card :options="options"></hm-balance-card>
  </div>
</template>
<script>
import HmBalanceCard from '@/components/hm-components/hm-balance-card/index.vue'

export default {
  components: { HmBalanceCard },
  data() {
    return {
      options: {
          layer:
            '/static/hm-balance-card/images/img_25821_0_0.png',
          info: '信用卡余额',
          zhanghaoguanli:
            '/static/hm-balance-card/images/img_25821_0_2.png',
          bd: '¥12929.05',
          main: '5326 5149 4497 1577',
          date: '日期',
          word: '12/24',
          cvv: 'CVV',
          num: '235',
          largeIcon:
            '/static/hm-balance-card/images/img_25821_0_1.png'
        }
    };
  },
  methods: {
    onClick: function(e) {
      console.log('onClick');
    }
  }
};
</script>
<style>
</style>

```

## 属性说明

| 属性名        | 类型     | 默认值 | 说明                                                                       |
|-----------   |---------|--------|----------------------------------------------------------------------------|
| options        | Object  | -      | 卡片属性                                                                   |

options对象各个属性说明如下：

| 属性名        | 类型     | 默认值 | 说明                                                                       |
|-----------   |---------|--------|----------------------------------------------------------------------------|
| layer        | String  | -      | 图片                                                                   |
| info        | String  | -      | 卡类型                                                                   |
| zhanghaoguanli        | String  | -      | 状态图片                                                                   |
| bd        | String  | -      | 余额                                                                   |
| main        | String  | -      | 卡号                                                                   |
| word        | String  | -      | 日期                                                                   |

## 事件说明

| 事件称名   | 事件说明           | 返回参数 |
|----------|--------------------|----------|
| @click   | 点击 Card 触发事件 | -        |

## 更新日志

### 0.0.1(2020-03-28)

* 完成第一个版本
