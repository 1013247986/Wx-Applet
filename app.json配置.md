##window配置

```markdown
    navigationBarBackgroundColor  导航栏背景颜色 不支持英文单词
    
    navigationBarTextStyle   导航栏标题颜色 进支持 black / white 两种颜色
    
    navigationBarTitleText   导航栏标题文字内容
    
    navigationStyle     导航栏样式 仅支持 default(默认样式) custom(自定义导航栏 只保留右上角     胶囊按钮)
    
    backgroundColor     窗口的背景色
    
    backgroundTexrStyle   下拉 loading的样式 仅支持 dark/light
    
    backgroundColorTop   顶部窗口的背景色，仅 iOS 支持
    
    backgroundColorBottom    底部窗口的背景色，仅 iOS 支持
    
    enablePullDownRefresh    是否开启当前页面的下拉刷新。
    
    onReachBottomDistance    页面上拉触底事件触发时距页面底部距离，单位为px。
    
    pageOrientation     屏幕旋转设置，支持 auto / portrait / landscape
```

##tabBar设置底部导航

color　　　　　　　　tab上的文字默认颜色

selectedColor 　　tab上的文字选中是的颜色

backgroundColor　　tab的背景色

borderStyle　　　　tabBar上版块的颜色 　　仅支持 black(黑色)/white(白色)

position　　　　　　可选值 bottom、topcustom　　　　　　　自定义tabBar

list　　　　　　　　tab的列表 最少2个 最多5个

　　list接受的是一个数组
　　　　属性　　　　　　　　　　描述
　　　　pagePath　　　　　　页面路径，必须在pages中先定义
　　　　text　　　　　　 　　tab上按钮文字
　　　　iconPath　　　　　　图片路径，icon大小限制为40kb 建议尺寸为81px*81px 不支持网络图片
　　　　selectedIconPath　选中的图片路径。当position 为top是，不显示icon

```js
示例 : "tabBar": {
  "list": [
   {
    "pagePath": "pages/index/index",
    "text": "首页"
   },
   {
    "pagePath": "pages/tab/index",
    "text": "日志"
   },
   {
    "pagePath": "pages/shopping/index",
    "text":"设置"
   }
  ],
  "custom": true,
  "color": "#fff",
  "selectedColor": "#000000",
  "backgroundColor": "red"
 }
```

