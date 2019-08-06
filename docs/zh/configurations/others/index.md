## 前端需要注意哪些 SEO?

### 创建唯一且准确的网页标题 title

title 标记可告诉用户和搜索引擎特定网页的主题是什么。它应放置在 HTML 文档的 head 元素中。我们应该为网站上的每个网页创建一个唯一标题，并且尽量避免与网页内容无关或使用默认或模糊的标题。如：

```html
<!-- 正确示范 -->
<title>前端搜索引擎优化的技巧</title>

<!-- 错误示范 -->
<title>我的文档</title>
```

### 使用 meta 元标签

我们可以使用 meta  的 keywords 元数据来提炼网页重要关键字，以及 description 元数据准确总结网页内容，而避免在 description 元数据的内容中出现关键词的堆砌，描述过长，或“这是一个网页”这种没有实际性意义的描述等现象。正确示范如下：

```html
<meta name='keywords' content='SEO,title,meta,语义化,alt'>
<meta name='description' content='介绍搜索引擎优化的技巧，如使用创建title标题、meta关键词和描述、语义化标签、img的alt属性等。'>
```

### 使用语义化元素

在合适的位置使用合适的元素表达合适的内容，让用户和“蜘蛛”能一目了然文档结构。例如使用 h1 可以让“蜘蛛”知道这是很重要的内容。然而，值得注意的是，例如在想要表达强调时，我们不应该滥用标题元素或者 b 、 i 这种没有实际意义的标签，换而可以使用 em 或 srtong 来表示强调。此外，h1 的权重比 h2 的大，我们不应该为了增大权重而去滥用 h1 ，一般来说 h1 用于正文的标题。

### 利用 <img> 中的 alt 属性

alt 属性可以在图片未成功显示时候，使用文本来代替图片的呈现，使“蜘蛛”可以抓取到这个信息。此外它还可以解决浏览器禁用图像或屏幕阅读器解析等问题。

### 设置rel='nofollow' 忽略跟踪

如果某个 a 的链接不需要跟踪，那么添加 rel='nofollow' 即可通知“蜘蛛”忽略跟踪。因为“蜘蛛”分配到每个页面的权重是一定的，为了集中网页权重并将权重分给其他必要的链接，为不必跟踪的链接添加这个属性就显得很必要了。

### 尽量保证 HTML 的纯粹和高质量

我们应尽量让结构（HTML）、表现（CSS）及行为（JavaScript）三者分离。如果在一个 HTML 页面中，编写大量的 CSS 样式或脚本，会拖慢其加载速度，此外，如果不为 img 定义宽高，那么会引起页面重新渲染，同样也会影响加载速度。一旦加载超时，“蜘蛛”就会放弃爬取。如果这个 HTML 文档内容比较独特丰富（合理插入图片说明）等，会被认为质量较高符合用户需求，从而提高 SEO 的排名。

### 扁平化网站结构

一般来说，一个网站的结构层次越少，越有利于“蜘蛛”的爬取。所以目录结构一般不多于 3 级，否则“蜘蛛”很容易不愿意继续往下爬。就像用户在操作一个网页一样，层级大于 3 就很影响用户体验了，“蜘蛛”就是模仿用户的心理。

### 合理安排重要内容的位置

我们应该将重要内容的 HTML 代码放在最前面，最前面的内容被认为是最重要的，优先让“蜘蛛”读取，进行内容关键词抓取。并且，重要内容不应该由 JavaScript 或 iframe 输出，“蜘蛛”没有办法读取 JavaScript ，一般不会去读取 iframe 中的内容。

## 请谈一下你对网页标准和标准制定机构重要性的理解。

网页标准和标准制定机构都是为了能让web发展的更‘健康’，首先约束浏览器开发者遵循统一的标准，其次约束网站开发者，这样降低开发难度，开发成本，SEO也会更好做，也不会因为滥用代码导致各种BUG、安全问题，最终提高网站易用性。

## 常见 web 安全及防护原理？

### sql注入原理

### XSS原理及防范

Xss(cross-site scripting)攻击指的是攻击者往Web页面里插入恶意 html标签或者javascript代码。

### XSS与CSRF有什么区别吗？

XSS是获取信息，不需要提前知道其他用户页面的代码和数据包。CSRF是代替用户完成指定的动作，需要知道其他用户页面的代码和数据包。

### HTTP和HTTPS

HTTP协议通常承载于TCP协议之上，在HTTP和TCP之间添加一个安全协议层（SSL或TSL），这个时候，就成了我们常说的HTTPS。

默认HTTP的端口号为80，HTTPS的端口号为443。

### 为什么HTTPS安全

因为网络请求需要中间有很多的服务器路由器的转发。中间的节点都可能篡改信息，而如果使用HTTPS，密钥在你和终点站才有。https之所以比http安全，是因为他利用ssl/tsl协议传输。它包含证书，卸载，流量转发，负载均衡，页面适配，浏览器适配，refer传递等。保障了传输过程的安全性。

