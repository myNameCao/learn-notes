# http 权威指南 
 
  +  url 提供了一种定位英特网上任意资源的手段，这些资源时可以通过各种不同的方案来访问的
  +  uri  有两种形式 一种是 URL 和URN
  +  URL  统一资源定位符 URN 统一资源名
**< scheme>://< user>:< password>@< host>:< port>/< path>;< params>?< query>#< frag>**
 
主要的是方案（scheme） 主机（host） 路径（path）  
  
  + 方案：访问服务器以获取资源使用的是那种协议
  + 主机： 主机名或者是点分ip地址 ，标示了英特网上能够访问资源的宿主机器
  + 端口：资源宿主服务器的正在监听的端口号 很多方案都有默认的端口号http 默认的端口号是80 
  + 路径：服务器上资源的本地名 由一个斜杠（/）将其与前面的url组件分隔开来；
  + 参数： 参数为名值对URL 中可以包含 多个参数字段 他们相互之间以及路径的其余部分之间用分号（；）分隔
  + 查询： 用字符？将其与URL的其余部分分隔开来
  + 片段：通过字符# 将其余URL的其余部分分隔开来 
  
 #### http 报文
 
 + 如果说http是因特网的信使 那么http 报文就是它搬用东西的包裹
 + http 报文是简单的格式化数据块，每条报文都包含一条客户端的请求或者一条来自服务器的响应，他们都是三个部分组成
 + 起始行：对报文进行描述，首部：包含属性 主体：可选的 包含数据。Content-type 行说明了主体是什么  content_length 说明了主体有多大
 + http 报文都可以分为两类：请求报文和响应报文；请求报文会向web 服务器请求一个动作，响应报文将请求的结果返回给客户端
 + 请求报文：包含   **方法** **请求的URL** **版本** 
 + 响应的报文： 包含 **状态码** **原因短语**  
 
 #### 求报文的方法：
 + GET  从服务器获取一份文档 
 + HEAD 只从服务器获取文档的首部 
 + POST 向服务器发送需要处理的数据
 + PUT  将请求的主体部分存储在服务器上 
 + TRACE 对可能经过的代理服务器传送到服务器上去的报文进行追踪 
 + OPTIONS 决定可以在服务器上执行那些方法 
 + DELETE 从服务器上删除一份文档
 
#### 常见的状态码  
+ 1xx 请求成功接受，继续处理
+ 200-206  成功 
+ 301 重定向（资源永久移动）
+ 302 资源暂时移动
+ 400 语法错误 不能被理解
+ 401 未授权
+ 403 服务器接到请求，但拒绝服务
+ 404 为找到    
+ 503 服务器现在无法为请求提供服务。但将来可以 


