# 1API 中转站 | GPT Claude Gemini API 代理 | OpenAI 兼容

> 聚合主流 AI 模型 API，降低 API 调用成本，支持 Cherry Studio、Lobe Chat 即插即用。

[![OpenAI Compatible](https://img.shields.io/badge/OpenAI-Compatible-brightgreen)](https://platform.openai.com/docs/api-reference/chat)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

## 关键词

GPT API 代理 | Claude API 中转 | Gemini Pro API | AI API 省钱 | OpenAI API 代理 | LLM API 转发 | ChatGPT API 便宜 | API Relay | AI Gateway | 自建 AI 渠道

---

## 什么是 1API 中转站？

1API 是一个 **AI 模型 API 中转服务**，帮助开发者以更低成本调用 GPT、Claude、Gemini 等主流大语言模型。所有接口兼容 OpenAI 格式，可直接对接 Cherry Studio、Lobe Chat、OpenCat 等主流客户端。

## 核心功能

- 🔄 **API 中转** — 统一接口，连接多个上游 API 渠道
- 💰 **成本优化** — 自建渠道，价格更便宜
- ✅ **新用户免费额度** — 注册即送免费测试额度
- 🔗 **OpenAI 兼容** — 主流客户端即插即用
- 🛡️ **智能路由** — 加权随机 + 失败自动重试（默认3次）
- 📊 **用量统计** — Token、请求次数、缓存命中率实时可见
- 🔑 **权限管理** — API Key 分组、模型限制、额度控制

## 支持的模型

| 模型 | 状态 |
|------|------|
| GPT-4o / GPT-4-turbo | ✅ 支持 |
| Claude 3.5 Sonnet / Haiku | ✅ 支持 |
| Gemini 1.5 Pro / Flash | ✅ 支持 |
| DeepSeek V3 | ✅ 支持 |
| Qwen (通义千问) | ✅ 支持 |
| 其他 OpenAI 兼容模型 | ✅ 支持 |

## 支持的客户端

| 客户端 | 配置难度 |
|--------|---------|
| [Cherry Studio](https://cherrystudio.com/) | ⭐ 一键导入 |
| [AionUI](https://aionui.app/) | ⭐ 一键导入 |
| [Lobe Chat](https://lobechat.com/) | ⭐ 手动配置 |
| [OpenCat](https://opencat.app/) | ⭐ 团队接入 |
| [DeepChat](https://deepchat.com/) | ⭐ 一键安装 |
| OpenAI API 兼容应用 | ✅ 通用 |

## 快速开始

### 1. 获取 API Key

访问 **[ctoai.xyz](http://ctoai.xyz)**，注册账号后在仪表盘创建 API Key。

### 2. 配置客户端

在支持 OpenAI API 格式的客户端中填入以下配置：

```
Base URL:  http://ctoai.xyz/v1
API Key:   你创建的 Key
```

### 3. 开始使用

```bash
# OpenAI 兼容格式调用示例
curl http://ctoai.xyz/v1/chat/completions \
  -H "Authorization: Bearer 你的Key" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "gpt-4o",
    "messages": [{"role": "user", "content": "你好"}]
  }'
```

## 价格

- ✅ **新用户有免费额度**，注册即可试用
- 💰 **价格便宜**，比官方渠道更省钱
- 📋 具体费率请登录 [ctoai.xyz](http://ctoai.xyz) 管理后台查看

## 常见问题

### Q: 如何获取 API Key？
A: 登录 [ctoai.xyz](http://ctoai.xyz)，进入「仪表盘」→「API Key」页面，点击「创建 Key」生成。

### Q: 额度怎么计算？
A: 按实际消耗计算，包括输入 Token + 输出 Token 合计、请求次数、缓存命中抵扣。

### Q: 通道失效/请求失败怎么办？
A: 中转站内置智能路由功能，配置多个通道时自动负载均衡，请求失败自动重试（默认重试3次）。

### Q: 支持哪些调用格式？
A: 完全兼容 OpenAI Chat Completions、Embeddings、Images、Audio 等 API 格式。

### Q: 可以用于商业项目吗？
A: 请确保上游 API 服务商允许商业使用，并遵守其服务条款。

## 技术栈

基于开源项目 [New API](https://github.com/QuantumNous/new-api) 构建。

## 相关链接

- 🌐 服务地址：[ctoai.xyz](http://ctoai.xyz)
- 📦 GitHub 源码：[github.com/jiafeimao0p/ctoai-docs](https://github.com/jiafeimao0p/ctoai-docs)
- 💬 技术讨论：[New API 官方仓库](https://github.com/QuantumNous/new-api/discussions)

---

*如果你觉得这个服务有用，欢迎 Star ⭐ 支持*