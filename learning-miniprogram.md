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

pages | window | tabBar | networkTimeout | debug 
--- | --- | --- | --- | --- 
设置页面路径 | 设置默认页面的窗口表现 | 设置底部tab的表现 | 打打打设置网络超时时间 | 设置是否开启debug模式


#### 2. WXML模板
#### 3. WXSS样式
#### 4. JS逻辑交互