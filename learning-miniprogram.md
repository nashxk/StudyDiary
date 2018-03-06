## 代码构成
#### 1. JSON配置
1. app.json: 小程序全局配置<br>
    [app.json](https://mp.weixin.qq.com/debug/wxadoc/dev/framework/config.html)
    
```json
{
  "pages": [
    "pages/index/index",
    "pages/logs/index"
  ],
  "window": {
    "navigationBarTitleText": "Demo"
  },
  "tabBar": {
    "list": [{
      "pagePath": "pages/index/index",
      "text": "首页"
    }, {
      "pagePath": "pages/logs/logs",
      "text": "日志"
    }]
  },
  "networkTimeout": {
    "request": 10000,
    "downloadFile": 10000
  },
  "debug": true
}
```

#### 2. WXML模板
#### 3. WXSS样式
#### 4. JS逻辑交互