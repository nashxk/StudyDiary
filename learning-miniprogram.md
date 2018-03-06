## 代码构成
### 1. JSON配置
- app.json: 小程序全局配置<br>
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
  设置页面路径 | 设置默认页面的窗口表现 | 设置底部tab的表现 | 设置网络超时时间 | 设置是否开启debug模式
  ---
  - pages
  > 数组的第一项代表小程序的初始页面。<br>
  文件名不需要后缀，框架自动寻找路径下**.json**, **.js**, **.wxml**, **.wxss**进整合
  ---
  - window
  属性 | 类型 | 默认值 | 描述
  --- | --- | --- | ---
  navigationBarBackgroundColor | HexColor | #000000 | 导航栏背景颜色
  navigationBarTextStyle | String | white | 导航栏标题颜色，black/white
  navigationBarTitleText | String | | 导航栏标题文字内容
  navigationStyle | String | default | 导航栏样式
  backgroundColor | HexColor | #ffffff | 窗口的背景色
  backgroundTextStyle | String | dark | 下拉背景字体、loading图的样式，dark/light
  enablePullDownRefresh | Boolean | false | 是否开启下拉刷新
  onReachBottomDistance | Number | 50 | 页面上拉触底时间触发时距页面底部距离，px

  ---
  - tabBar
  
  ---
  - networkTimeout
  ---
  - debug 
  ---

- page.json: 页面的json文件，只能设置window的相关配置项
- project.config.json: 

### 2. WXML模板

  [WXML](https://mp.weixin.qq.com/debug/wxadoc/dev/framework/view/wxml/)
  充当HTML的角色

### 3. WXSS样式
  
  [WXSS](https://mp.weixin.qq.com/debug/wxadoc/dev/framework/view/wxss.html)
  充当CSS
### 4. JS逻辑交互