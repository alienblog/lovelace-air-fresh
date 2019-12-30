# 米家新风机的HASS卡片

  适配 [HACS新风机插件](https://github.com/alienblog/mi-airfresh)

```
// 引入
resources:
  - type: js
    url: /community_plugin/lovelace-air-fresh/air-fresh.js


// 使用面板卡
type: 'custom:air-fresh'
entity: fan.xiaomi_miio_device


// 使用面板卡（自定义背景图片）
// background-image 设置图片地址
// background-size 设置图片显示模式（别改）
// background-position 设置图片偏移量（x轴 y轴）

type: 'custom:air-fresh'
entity: fan.xiaomi_miio_device
style: >-
  .air-fresh-panel{
    background-image: url(https://i1.mifile.cn/f/i/16/chain/fresh-air-ventilator/fresh-16-2.jpg);
    background-size: cover;
    background-position: -10px 0;
  }

```

![](01.png)

## 更新
+ 修复了卡片冲突的问题
+ 优化了显示效果
