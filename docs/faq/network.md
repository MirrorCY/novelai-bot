# 插件相关

## 功能相关

### 使用这个插件必须花钱吗？

如果你用默认配置，那么是需要的。你也可以选择自己搭建服务器或使用 colab 等，这些方案都是免费的。

## 网络相关

### 请求超时

如果偶尔发生无需在意。如果总是发生请尝试调高 `requestTimeout` 的数值或者配置 `proxyAgent`。

### 未知错误 401

请确认 `type` 是否设置为 `token`。

将 `type` 切换成 `login` 后重载，再次切换成 `token` 重载可以解决此问题。

### 未知错误 404

请确认 `endpoint` 是否正确，以及版本是否是最新。

### 未知错误 503

请尝试将 `endpoint` 中的 `api` 替换成 `backend-production-svc`。