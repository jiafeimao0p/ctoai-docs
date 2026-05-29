# 1API 中转站

聚合主流 AI 模型，统一 API 接口，降低使用成本。

## 功能特性

- **多渠道管理** — 支持配置多个上游 API 通道
- **智能路由** — 加权随机 + 失败自动重试
- **OpenAI 兼容** — 支持 Cherry Studio、Lobe Chat、OpenCat 等客户端即插即用
- **用量统计** — Token 消耗、请求次数、缓存命中率实时可见
- **权限管理** — API Key 分组、模型限制、额度控制

## 支持的模型

GPT-4o、GPT-4-turbo、Claude 3.5、Gemini 1.5、DeepSeek V3、Qwen 等主流模型。

## 支持的客户端

| 客户端 | 配置方式 |
|--------|---------|
| Cherry Studio | 一键导入 |
| AionUI | 一键导入 |
| Lobe Chat | 手动配置 |
| OpenCat | 团队接入 |
| DeepChat | 一键安装 |

## 价格

- ✅ **新用户有免费额度**
- 💰 **价格便宜**，自建渠道更省钱
- 具体费率请登录管理后台查看

## 快速开始

### 第一步：获取 API Key

登录 [ctoai.xyz](http://ctoai.xyz)，在仪表盘或设置页面创建你的 API Key。

### 第二步：配置客户端

通用配置：

```
Base URL:  http://ctoai.xyz/v1
API Key:   你的Key
```

### 第三步：开始使用

兼容 OpenAI 格式的主流模型调用，包括 Chat Completions、Embeddings、Images、Audio 等。

## 请求示例

```bash
curl http://ctoai.xyz/v1/chat/completions \
  -H "Authorization: Bearer 你的Key" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "gpt-4o",
    "messages": [{"role": "user", "content": "你好"}]
  }'
```

## 常见问答

**Q1：如何获取 API Key？**
登录 ctoai.xyz，进入仪表盘或设置页面，点击「创建 Key」即可。

**Q2：额度怎么算？**
额度按实际消耗计算，包括输入+输出 Token 合计、请求次数、缓存命中抵扣。

**Q3：通道失效怎么办？**
中转站内置智能路由功能，配置多个通道时自动负载均衡，请求失败自动重试（默认3次）。

**Q4：支持哪些客户端？**
支持 Cherry Studio、AionUI、Lobe Chat、OpenCat、DeepChat 等主流客户端。

## 注意事项

- 请通过正规途径获取上游 API Key
- 遵守上游服务商的使用条款
- 公开提供生成式 AI 服务需符合当地法规要求

## 技术栈

基于 [New API](https://github.com/QuantumNous/new-api) 构建。

## 联系方式

服务地址：[ctoai.xyz](http://ctoai.xyz)