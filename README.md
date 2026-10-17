# proxyip-api

edgetunnel (cmliu) 两用优选 API（cfdata 本地优选产出）。

## 接入
worker 的 KV `ADD.txt`（或 /admin 优选订阅生成器）加一行：

```
https://raw.githubusercontent.com/0Rita18/proxyip-api/main/results/ip.txt?proxyip=true#ProxyIP两用
```

`?proxyip=true`：worker 拉取时把本批 ip:port 同时进「优选入口 + 反代IP池」（请求优选API() → 反代IP池.add）。
