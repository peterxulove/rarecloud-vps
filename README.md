# RareCloud VPS 全产品线推荐与选购指南

把 RareCloud（rarecloud.io）官网在售的 **19 个可下单套餐**逐款拆开：配置在什么级别、
支持几个付款周期、月均价折算下来是多少、机房在哪、硬件是什么型号，以及 NodeSeek 社区的真实评价
——**包括它的续费涨价、强制迁移换 IP 和退款难这些槽点**。

## 页面

| 文件 | 说明 |
|------|------|
| [`rarecloud-vps-guide.html`](rarecloud-vps-guide.html) | 主页面（单文件，含 JSON-LD 结构化数据；每个价格单元格均为 aff 购买链接） |
| [`rarecloud-vps-guide.md`](rarecloud-vps-guide.md) | 同一内容的 Markdown 版；每个价格均附 aff 购买链接 |
| [`index.html`](index.html) | 首页跳转页（`/` → `rarecloud-vps-guide.html`） |
| [GitHub Pages 预览](https://peterxulove.github.io/rarecloud-vps/rarecloud-vps-guide.html) | 在线选购指南 |
| [Google Sites 预览](https://sites.google.com/view/rarecloud-vps) | Google Sites 镜像页 |

## RareCloud 推广购买入口（aff=1012）

以下为 RareCloud 官方产品级推广链接。通过链接访问后购买，不会增加用户费用，
商家会按每次续费支付 15% 持续佣金。

| 产品线 | 套餐 | 最低月均价 | 最便宜周期 | 推广购买链接 |
|--------|------|------------|------------|--------------|
| Linux KVM VPS | Starter KVM | €2.08/月 | 三年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=3) |
| Linux KVM VPS | Micro KVM | €1.56/月 | 三年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=6) |
| Linux KVM VPS | Advanced KVM | €3.89/月 | 三年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=11) |
| Linux KVM VPS | Core VPS | €3.19/月 | 三年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) |
| Linux KVM VPS | Plus VPS | €7.92/月 | 半年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) |
| Linux KVM VPS | Pro VPS | €16.25/月 | 半年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) |
| Linux KVM VPS | Elite VPS | €25.00/月 | 三年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=15) |
| Linux KVM VPS | Do It Yourself VPS | €6.25/月 | 半年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=16) |
| Windows RDP VPS | Win 4G | €12.92/月 | 年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=7) |
| Windows RDP VPS | Win 8G | €24.58/月 | 年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=17) |
| Windows RDP VPS | Win 12G | €28.75/月 | 年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=18) |
| 应用预装 VPS | N8N Starter | €4.00/月 | 年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=36) |
| 应用预装 VPS | N8N PRO | €5.69/月 | 年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=37) |
| 应用预装 VPS | OpenClaw Server | €4.00/月 | 年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=49) |
| 应用预装 VPS | OpenClaw Desktop | €5.69/月 | 年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=50) |
| Web 虚拟主机 | StartUp | €7.92/月 | 年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=21) |
| Web 虚拟主机 | Business | €16.25/月 | 年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=22) |
| Web 虚拟主机 | Enterprise | €16.25/月 | 两年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=23) |
| Web 虚拟主机 | Website Hosting | €2.22/月 | 三年付 | [下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=51) |

## 内容结构

速览结论 → 19 个套餐与真实月均价 → 12 个数据中心（机房 / ASN / 上游 / IX / test IP）→
大陆三网 × 机房适配矩阵 → 逐条产品线详解（含 Cloud VM 13 规格与云附加件）→
NodeSeek 社区真实评价 → 6 条风险提示 → 常见问题 → 数据来源。

## 核心结论

- **谁在运营**：罗马尼亚 RARE MOOD AGENCY SRL（Tax ID 45192771，VAT RO45192771），
  背后是持牌运营商 **M247（AS9009）**；12 个机房中 7 个直接挂在 M247 的 AS9009 下
- **最低价**：€1.56/月（Micro KVM，1C/768M/15G NVMe/1T，**一次付三年 €56**）
- **三条价格规则**：Micro / Starter / Website Hosting **没有月付**；
  Plus / Pro / Elite / Win 系列**两年付与三年付同价**（锁三年没折扣）；
  所有价格**不含 VAT**（欧盟无 VAT ID 加 19%）
- **大陆选机房**：移动选**香港**（移动快乐鸡，回程 CMI 直连）；
  电信 / 联通选**德国**（回程 4837 直连，延迟约 180–260ms）；
  **电信不要选香港 / 东京**（回程绕路、丢包）
- **五个坑**：① 2026-09 已通知续费涨价；② 2025-12 荷兰强制迁移，退役 3 个 /24 并全部换 IP；
  ③ 充值赠金只有 60 天有效期、续费一次只能消耗一个周期；④ 14 天退款政策实际很难执行，
  社区共识是「用 PayPal 付、走 PayPal 争议」；⑤ 条款明确**不做数据备份**、IP 不可迁移

## 数据来源

- 产品与价格：RareCloud 官网 WHMCS 导出（`https://rarecloud.io/data/whmcs-pricing.json`，
  last_updated 2026-10-14 04:00:01）；
  机房数据来自官网 12 个数据中心页；条款与联盟政策来自官网 TOS / affiliates 页
- 第三方测评：NodeSeek 搜索「rarecloud」9 页共 417 条结果中，按评论数排序取前 200 篇 +
  补抓 2 篇，共 202 篇正文与 1761 条评论
- 采集方式：本机 Chrome 登录态 + CDP（bsk）

> 价格与库存为抓取时点快照，随时可能变动；以官网实时信息为准。
> 本文含推广链接，不构成购买建议，请结合自身风险承受能力判断。
