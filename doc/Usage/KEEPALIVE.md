# 功能介绍: KEEPALIVE模式

## Docker/Hugging Face Space/Node.js

在网页设置中开启`KEEPALIVE`开关，可以启用KEEPALIVE响应模式。

启用KEEPALIVE模式后，使用流式请求到脚本，脚本会持续向客户端发送心跳响应以保持客户端的持续连接，防止客户端发生异常断开的情况。

注意，当使用`KEEPALIVE`功能时，请确保使用的请求密钥(Worker Api Key)的安全设定为关闭(Disabled)，且在请求时使用流式响应。
`KEEPALIVE`功能不会影响到非流式响应或启用了安全设定的流式响应。

