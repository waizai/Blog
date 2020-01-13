# bridge原理



h5: 注入jsbridge, 把相关的方法挂载到window上,
调用相关功能、通知 Native 当前 JS 的相关状态等。
1. h5调起native: 
    a. 注入
    b. 拦截scheme
2. h5通知native: 

Native: 
回溯调用结果、消息推送、通知 JS 当前 Native 的状态等
1. native向h5发送消息： 
2. naive通知h5: 


容器
1. WebView
2. JSCore

#### h5调用native
1. Android
<!-- nativeBridge: scheme -->
<!-- myJavaScriptInterface： 代理类，包含了逻辑部分-->
<!-- addJavascriptInterface: 是webview的一个方法 -->
Wv.addJavascriptInterface(myJavaScriptInterface, "nativeBridge");

<!-- 前端调用 -->
window.nativeBridge.postMessage(message);

2. IOS
<!-- 注入对象，前端调用其方法时，Native 可以捕获到 -->
<!-- userCC: WKUserContentController-->
[userCC addScriptMessageHandler:self name:@"nativeBridge"];

<!-- 前端调用：  -->
window.webkit.messageHandlers.nativeBridge.postMessage(message);

#### native调用h5

1. Android
webView.loadUrl("javascript:" + javaScriptString);

2. IOS
a. UIWebView
result = [uiWebview stringByEvaluatingJavaScriptFromString:javaScriptString];

b. WKWebView
[wkWebView evaluateJavaScript:javaScriptString completionHandler:completionHandler];


