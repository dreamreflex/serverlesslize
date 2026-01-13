# Serverlesslize （s12e）

无服务化转型是应用[《AI驱动的边缘应用转型白皮书》](https://doc.dreamreflex.com/legal/%E9%A1%B9%E7%9B%AE%E7%99%BD%E7%9A%AE%E4%B9%A6/AI%E9%A9%B1%E5%8A%A8%E5%BA%94%E7%94%A8%E9%A1%B9%E7%9B%AE%E7%99%BD%E7%9A%AE%E4%B9%A6.html)中要求的一种探索方向，核心内容是将传统的云应用，云原生应用，Docker应用逐步转向无服务器应用，函数应用。

## 原则

s12e的转型原则是“能转则转，能改则改，能优则优”

上述原则指的是如何一个应用能够进行完全Serverless化，那么就试着进行完全转型。如果一个应用能够部分改造为Serverless应用，那么就进行部分改造，例如前后端应用中的前端通常是SPA，SPA的构建打包通常是纯静态构件，而纯静态构建可以被改造成Serverless的。能优则优指的是如果一个应用无法改造，那就试着从优化的角度进行应用，例如利用他的转发防护功能抵挡DDoS工具，WAF和漏洞扫描等，降低安全防护成本。
## 相关项目

1. [EdgeOneKV存储抽象](https://github.com/phil616/s12e-edgeone-kv-interface) - 一个将KV存储抽象为HTTP的项目，s12e的原子能力之一
2. [EdgeBitwarden](https://github.com/phil616/s12e-EdgeBitwarden) - 一个Bitwarden的Serverless版本，利用EdgeOne KV作为后端存储，支持Passkey
3. [OAuthGateway](https://github.com/phil616/s12e-oauthgateway) - 一个利用边缘能力搭建的OAuth防护认证网关
4. [Mindmap脑图](https://github.com/phil616/s12e-mindmap) - 一个利用百度脑图项目进行边缘化处理的浏览器无服务器脑图工具


LICENSE CC4.0 & MIT
