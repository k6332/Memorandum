> shim和polyfill

#### 关系：shim > polyfile

>> Shim

Shim 指的是在一个旧的环境中模拟出一个新 API ，而且仅靠旧环境中已有的手段实现，以便所有的浏览器具有相同的行为。

特征：

* 该 API 存在于现代浏览器中;
* 浏览器有各自的 API 或 可通过别的 API 实现;
* API 的所有方法都被重新实现；
* 拦截 API 调用，并提供自己的实现；
* 是一个优雅降级。

>> Polyfill

polyfill 是一段代码(或者插件)，提供了那些开发者们希望浏览器原生提供支持的功能。程序库先检查浏览器是否支持某个API，如果不支持则加载对应的 polyfill。

特征:

* 是一个浏览器 API 的 Shim;
* 与浏览器有关;
* 没有提供新的API，只是在 API 中实现缺少的功能;
* 以只需要引入 polyfill ，它会静静地工作;