---
title: IFG GEO Optimizer
description: IFG GEO Optimizer Shopify 应用的文档、常见问题和法律页面。
lang: zh
---

# 隐私政策

<div class="lang-switcher">
{% include lang-switcher.html current="zh" slug="privacy" %}
</div>

**IFG GEO Optimizer** —— 一款用于生成式引擎优化的 Shopify 应用
最后更新：2026 年 7 月

## 1. 数据控制者

**IFG GEO Optimizer** 处理的个人数据的数据控制者为：

**IFG eCommerce** —— 总部位于意大利罗马
邮箱：[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. 我们收集的数据

- **商家账户数据（通过 Shopify OAuth）**：你的商店域名、一个 API 访问令牌，以及你 Shopify 账户上的邮箱地址。
- **目录数据（只读）**：产品标题、描述、供应商、价格、选项和技术规格——用于执行审计、模拟爬虫行为、评估内容可提取性得分，以及起草 FAQ 或重写描述。
- **商店配置信息**：你的当前套餐、你在“设置”中填写的退货和运费政策详情及公司数据、已保存的审计记录、FAQ 和内容重写草稿，以及你选择追踪的 AI 可见度提示语。
- **支持聊天消息**：你与应用内 AI 助手交流的文本内容，包括在你明确要求转接人工时转发给我们的对话记录。
- **匿名前台流量（Web Pixel，Grow/Unlimited）**：当访客从已识别的 AI 引擎（ChatGPT、Perplexity、Claude、Gemini、Copilot）访问产品页面时，我们会记录该引擎、页面 URL 和时间戳——仅在访客已通过你商店的 Cookie 横幅给予分析同意后才会记录。不会收集任何访客标识符、Cookie 或会话数据。
- **技术数据**：请求时间戳、内部记录标识符和系统日志。

> 应用**绝不会请求或接收个人终端客户数据**——没有姓名、邮箱、地址或订单信息。应用请求的 Shopify 权限为 `read_products`、`write_products`（目录和结构化数据）、`read_themes`（检查主题嵌入是否已激活）和 `write_pixels`（激活上述匿名流量像素）。

## 3. 我们处理数据的原因及法律依据

我们处理这些数据是为了提供你安装本应用所需的服务——依据 GDPR 第 6(1)(b) 条，即履行合同的需要：分析并改善你的目录在生成式搜索引擎上的可见度，包括 AI 辅助的 FAQ 起草和内容重写、应用内支持聊天、对你选择的提示语进行每周 AI 可见度追踪，以及匿名的 AI 引荐流量测量——所有这些要么由商家主动发起，要么（对于流量像素而言）在你的前台商店中受同意机制约束。

## 4. 我们如何收集数据

账户数据通过 Shopify 的 OAuth 流程在安装时一次性收集。目录数据仅在你从仪表盘触发操作时，通过 Shopify Admin API 读取。流量像素在你的前台商店运行，仅在获得同意后报告事件；除非你主动触发，否则不会有任何其他内容在后台运行。

## 5. 我们与谁共享数据

- **Google Firebase / Cloud Firestore** —— 存储你的配置、会话和草稿。Google LLC（美国）参与了欧盟-美国数据隐私框架（EU-US Data Privacy Framework）。数据存储在 europe-west1 区域（比利时）。
- **Anthropic PBC（美国）** —— 提供用于 FAQ 起草、内容重写和应用内支持聊天的 Claude 模型，仅在你明确操作时使用。仅接收你提供的产品属性或聊天文本——绝不接收客户数据。
- **OpenAI, Inc.（美国）** 和 **Perplexity AI, Inc.（美国）** —— 仅用于对你明确选择监控的提示语进行每周 AI 可见度追踪。仅接收被追踪的提示语文本——绝不接收客户数据。
- **Google LLC（美国）** —— 提供 Gemini 模型，用途与上述 OpenAI/Perplexity 在可见度追踪中的用途相同（与仅作为存储用途的 Firebase/Firestore 是不同的用途）。
- **Resend, Inc.（美国）** —— 仅在你在支持聊天中明确要求转接人工时，向我们发送包含商店名称和支持聊天记录的通知。
- **Shopify Inc.** —— 平台本身，也是应用所使用的 Admin API 和 Web Pixel 基础设施的来源。

我们不出售数据，也不将其用于营销或行为画像。

## 6. 我们的数据保留期限

- **会话令牌**：由 Shopify 的离线令牌生命周期管理，自动轮换。
- **配置信息、审计记录、草稿和流量事件**：在应用安装期间持续保留。卸载会触发 Shopify 的 `shop/redact` webhook，彻底删除你商店的配置信息和会话数据。
- **技术日志**：按照 Google Cloud 的标准日志保留策略保留。

## 7. 你的权利

依据 GDPR 第 15–22 条，你可以请求访问你的数据、更正不准确的数据，或要求删除——最简单的方式就是卸载应用——或反对数据处理。你也可以向当地数据保护机构投诉。由于本应用从不处理个人终端客户数据，`customers/data_request` 和 `customers/redact` 合规性 webhook 会返回确认信息，说明没有可导出或删除的数据。

## 8. 安全性

所有流量均通过 HTTPS/TLS 1.2+ 传输。Shopify 认证令牌绝不会暴露给浏览器。每个 webhook 在处理前都会经过恒定时间的 HMAC SHA-256 校验。数据库只能从后端访问，通过托管平台自身的服务身份进行认证——代码中没有静态凭据，数据库自身的安全规则也拒绝任何直接的客户端访问。数据在静态存储和传输过程中均经过加密。

## 9. 变更

我们可能会不时更新本政策。重大变更会在此处体现，页面顶部的日期会保持最新。

---

**对你的数据有疑问？**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← 返回帮助中心](index.html)
