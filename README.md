#### 1. WebView的加载和网络请求并行
> 所有的网络请求并不是从WebView内核发起request，而是启动WebView的过程中，我们通过native的渠道建立自己的HTTP链接，
然后从CDN和我们称作offlineServer的地方获取页面
