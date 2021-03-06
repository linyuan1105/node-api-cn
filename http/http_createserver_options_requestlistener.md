<!-- YAML
added: v0.1.13
changes:
  - version: v12.15.0
    pr-url: https://github.com/nodejs/node/pull/31448
    description: The `insecureHTTPParser` option is supported now.
  - version: v9.6.0, v8.12.0
    pr-url: https://github.com/nodejs/node/pull/15752
    description: The `options` argument is supported now.
-->

* `options` {Object}
  * `IncomingMessage` {http.IncomingMessage} 指定要使用的 `IncomingMessage` 类。用于扩展原始的 `IncomingMessage`。**默认值:** `IncomingMessage`。
  * `ServerResponse` {http.ServerResponse} 指定要使用的 `ServerResponse` 类。用于扩展原始的 `ServerResponse`。**默认值:** `ServerResponse`。
  * `insecureHTTPParser` {boolean} 使用不安全的 HTTP 解析器，当为 `true` 时接受无效的 HTTP 请求头。应避免使用不安全的解析器。有关更多信息，参阅 [`--insecure-http-parser`]。**默认值:** `false`。
* `requestListener` {Function}
* 返回: {http.Server}

返回新的 [`http.Server`] 实例。

`requestListener` 是一个自动添加到 [`'request'`] 事件的函数。


