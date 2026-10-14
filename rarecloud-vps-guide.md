---
title: RareCloud VPS 全产品线推荐与选购指南：19 个套餐、12 个数据中心、配置价格与运营商适配（2026）
description: RareCloud（rarecloud.io）VPS 选购指南：逐款拆解 19 个可下单套餐——Linux KVM VPS 8 档、Windows RDP VPS 3 档、n8n 与 OpenClaw 预装 VPS 4 档、Web 虚拟主机 4 档，以及布加勒斯特 Cloud VM 的 13 个规格；给出 12 个数据中心的机房 / ASN / 上游 / test IP、大陆电信联通移动的选点建议、NodeSeek 社区真实评价与续费涨价、迁移换 IP、退款难等风险提示。
date: 2026-10-14
source: rarecloud-vps-guide.html
---

# RareCloud VPS 全产品线推荐与选购指南

把 RareCloud（rarecloud.io）官网在售的 **19 个可下单套餐**逐款拆开：配置是什么、支持哪几个付款周期、
折合每月到底多少钱、12 个数据中心分别在哪、大陆电信 / 联通 / 移动该怎么选机房，以及 NodeSeek 社区的真实评价怎么说
——**包括它的续费涨价、强制迁移换 IP 和退款难这些槽点**。

产品与价格数据整理自 RareCloud 官网（rarecloud.io，WHMCS 定价导出 2026-10-14 04:00:01）· 测评引用来自 NodeSeek 社区 · 更新于 2026-10-14

> **请先阅读：**本文是产品整理与选购参考，**不是 RareCloud 官方文档**。价格、库存、线路随时可能调整，
> 下单前请以官网页面为准。文中的购买链接包含推广参数（aff），通过该链接下单不会增加你的费用。
> **本文同样列出了该商家被社区质疑的问题**，请务必看完「选购注意事项与风险提示」再决定。
> 文末列出全部引用来源，可自行复核。

目录

1. [一分钟选型结论](#quick)
2. [全部套餐速览表](#matrix)
3. [按运营商 / 机房选](#isp)
4. [12 个数据中心与 test IP](#dc)
5. [Linux KVM VPS（8 档）](#linux)
6. [Windows RDP VPS（3 档）](#windows)
7. [n8n 自动化 VPS（2 档）](#n8n)
8. [OpenClaw AI 助手 VPS（2 档）](#openclaw)
9. [Web 虚拟主机（4 档）](#hosting)
10. [Cloud VM 与云附加件（13 规格）](#cloud)
11. [全部 19 个套餐与推广入口](#allplans)
12. [社区口碑：被认可与被吐槽](#voice)
13. [常见问题](#faq)
14. [选购注意事项与风险提示](#caveats)
15. [数据来源与引用](#sources)

## 一分钟选型结论

RareCloud 的产品骨架可以用一句话概括：**11 个机房 × 5 条产品线 × 19 个固定套餐**，
再加一套**按小时计费的 Cloud VM**。这里最关键的选择不是产品线而是**机房**——它决定了你的回程走哪条线路。

| 你的情况 | 推荐套餐 | 产品线 | 参考价格 / 购买 | 核心理由 |
| --- | --- | --- | --- | --- |
| 预算压到最低，能一次付 3 年 | [Micro KVM](#linux) | Linux KVM VPS | [€1.56/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=6) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=6) | 1 vCPU / 768MB / 15GB NVMe / 1TB 流量，全站最低价；缺点是只有年付及以上，且内存很小 |
| 想要一台正常能用的 Linux 小机 | [Core VPS](#linux) | Linux KVM VPS | [€3.19/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) | 1 vCPU / 2GB / 40GB NVMe / 3TB 流量，各周期都有，月付 €5.50 |
| 要 2 核 4GB 跑网站 / 服务 | [Plus VPS](#linux) | Linux KVM VPS | [€7.92/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) | 2 vCPU / 4GB / 65GB NVMe / 5TB 流量；注意它两年付与三年付同价，锁两年就够 |
| 要 4 核 8GB 的主力配置 | [Pro VPS](#linux) | Linux KVM VPS | [€16.25/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) | 4 vCPU / 8GB / 100GB NVMe / 7TB 流量，同样两年付与三年付同价 |
| 内存要拉满（16GB） | [Elite VPS](#linux) | Linux KVM VPS | [€25.00/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=15) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=15) | 4 vCPU / 16GB / 150GB NVMe / 10TB 流量，Linux 线唯一三年付还能再便宜一档的 |
| CPU / 内存 / 硬盘都不够，想自己配 | [Do It Yourself VPS](#linux) | Linux KVM VPS | [€6.25/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=16) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=16) | vCPU 1→8、内存 1→32GB、硬盘 20→500GB、流量 1→20TB 全自选，只有月付到年付 |
| 要跑 Windows 软件，团队远程桌面共用 | [Win 4G](#windows) | Windows RDP VPS | [€12.92/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=7) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=7) | 2 vCPU / 4GB / 60GB NVMe / 4TB；Windows 授权需自行购买，模板自带 180 天评估期 |
| 要自建 n8n 工作流，预算要低 | [N8N Starter](#n8n) | None | [€4.00/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=36) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=36) | 预装 n8n + Nginx + Let's Encrypt + UFW，年付 €48 折合 €4.00/月，全站年付折扣最猛 |
| 要自建 n8n，重工作流 / 高并发 | [N8N PRO](#n8n) | None | [€5.69/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=37) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=37) | Docker + PostgreSQL 16 + Redis 7 + 2 个 worker 节点，数据库与缓存不对公网暴露 |
| 要在自己服务器上跑 AI 助手（接 Telegram / 微信） | [OpenClaw Server](#openclaw) | None | [€4.00/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=49) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=49) | 预装 OpenClaw + headless Chrome，8 层安全加固，仪表盘只监听 localhost |
| 想看着 AI 实时点网页、填表单 | [OpenClaw Desktop](#openclaw) | None | [€5.69/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=50) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=50) | 4 vCPU / 8GB / 100GB，多一套 XFCE 图形桌面 + 非 headless 浏览器，可 VNC 观看 |
| 只想放个 WordPress / 静态站，不碰服务器 | [StartUp](#hosting) | Web 虚拟主机 | [€7.92/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=21) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=21) | 1 个网站 / 50GB NVMe / 不限流量 / 独立 IP / 免费 SSL / 每日备份 |
| 预算最低的建站方案 | [Website Hosting](#hosting) | Web 虚拟主机 | [€2.22/月 起](https://rarecloud.io/clients/aff.php?aff=1012&pid=51) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=51) | 10GB NVMe / 不限流量 / 10 个邮箱 / 送 .com 域名，年付 €30 起，没有月付 |
| 要按小时计费、随时删的云主机 | [Cloud VM S-1](#cloud) | Cloud VM | [€3.99/月 封顶](https://rarecloud.io/clients/aff.php?aff=1012) [购买](https://rarecloud.io/clients/aff.php?aff=1012) | 1 vCPU / 2GB / 25GB NVMe / 1TB 流量，按小时出账、月价封顶，只在布加勒斯特机房 |

> **三句话记住 RareCloud 的规则：**
>
> - **年付折算最便宜**，但最便宜的两档（Micro / Starter）**没有月付**，最低一次性付 1.5 年。
> - **移动选香港，电信 / 联通选德国，电信千万别选香港和东京**（回程绕路、丢包）。
> - **Plus / Pro / Win 系列的两年付与三年付同价**，锁三年零收益，最多锁两年。

## 全部套餐速览表

下表按产品线列出**各线最低档**的规格与价格，便于横向比较。完整档位见后文各产品小节。

| 产品线 | 最低档 | 配置 | 流量 | 计费周期 | 最低月均价 / 购买 |
| --- | --- | --- | --- | --- | --- |
| [Linux KVM VPS](#p-linux-kvm) | [Micro KVM](#p-linux-kvm) | 1 vCPU / 768MB RAM / 15GB NVMe | 1TB /month | 3 个可用周期 | [€1.56](https://rarecloud.io/clients/aff.php?aff=1012&pid=6) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=6) <small>（三年付，一次性付 €56.00）</small> |
| [Windows VPS](#p-windows-rdp) | [Win 4G](#p-windows-rdp) | 2 vCPUs / 4GB RAM / 60GB NVMe | 4TB /month | 4 个可用周期 | [€12.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=7) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=7) <small>（年付，一次性付 €155.00）</small> |
| [n8n VPS](#p-n8n) | [N8N Starter](#p-n8n) | 2 vCPU / 4GB RAM / 65GB NVMe | 5TB /month | 2 个可用周期 | [€4.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=36) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=36) <small>（年付，一次性付 €48.00）</small> |
| [OpenClaw VPS](#p-openclaw) | [OpenClaw Server](#p-openclaw) | 2 vCPU / 4GB RAM / 65GB NVMe | 5TB /month | 2 个可用周期 | [€4.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=49) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=49) <small>（年付，一次性付 €48.00）</small> |
| [Web 虚拟主机](#p-hosting) | [Website Hosting](#p-hosting) | 共享 / 共享 / 10GB NVMe | 不限流量 | 3 个可用周期 | [€2.22](https://rarecloud.io/clients/aff.php?aff=1012&pid=51) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=51) <small>（三年付，一次性付 €80.00）</small> |

价格均为官网标价的欧元数字（**不含 VAT**），未含任何优惠码与支付手续费。
年付款的档位会同时标注「一次性付总额」与「折合每月」，方便和月付直接比较。

## 按运营商 / 机房选

这是本文最实用的一张表。结论综合了官网机房页公布的上游与互联、NodeSeek 帖子的回程路由记录与评论。
星级含义：**★★★** 推荐 · **★★☆** 可用但有短板 · **★☆☆** 有明确负面反馈 · **—** 数据不足。

| 用户类型 | 中国香港 | 日本东京 | 德国 | 荷兰 / 英国 | 罗马尼亚 | 美国 |
|---|---|---|---|---|---|---|
| 中国联通 | ★★☆ | ★★☆ | ★★★ | ★★★ | ★★☆ | ★☆☆ |
| 中国电信 | ★☆☆ | ★☆☆ | ★★★ | ★★☆ | ★★☆ | ★☆☆ |
| 中国移动 | ★★★ | ★★☆ | ★★☆ | ★★☆ | ★★☆ | ★☆☆ |
| 教育网 CERNET | — | — | — | — | — | — |
| 欧洲业务 / 调用欧洲 API | ★★☆ | ★☆☆ | ★★★ | ★★★ | ★★★ | ★☆☆ |
| 美国业务 / 调用美国 API | ★★☆ | ★★★ | ★☆☆ | ★☆☆ | ★☆☆ | ★★★ |
| 流媒体解锁 | ★☆☆ | ★☆☆ | ★☆☆ | ★☆☆ | ★☆☆ | ★☆☆ |
| 建站 / 博客 / 落地页 | ★★★ | ★★☆ | ★★★ | ★★★ | ★★☆ | ★★☆ |

> **几个具体结论，直接抄作业：**
>
> - **移动用户优先选香港。** 香港机房回程 CMI 直连、部分地区命中 CMIN2 精品线路，社区反复称「移动快乐鸡」；但有一篇晚高峰测评显示北方移动仍会混入 4837，河北 388ms / 山西 372ms / 辽宁 503ms，晚高峰丢包并不低。
> - **电信用户选德国，不要选香港和东京。** 香港回程被实测判定为「英国 → 欧洲 → 香港 → 美国 → 北京」（AS9009 → AS3356 → AS4837 → AS4808），丢包且延迟高；日本机房电信方向也被多次提到绕路。
> - **联通用户选德国或荷兰。** 德国回程走联通 4837，延迟低于 200ms；荷兰（海牙）迁站后也被用户称为「联通快乐」。
> - **流媒体解锁全线别指望。** 有用户直接反馈「不要指望解锁，广播 IP，Gemini 给你飞罗马尼亚，chatgpt 直接显示你是 VPN」。需要干净 IP 请另找专门商家。
>
> 机房是**下单时选**的，每个套餐都能落在 11 个 VPS 机房中的任意一个 —— 同
> 一个套餐选德国和选香港是同一个 pid，只是线路不同。

## 12 个数据中心与 test IP

RareCloud 用的是**批发型网络**：自营 Tier III 机房 + Tier-1 出口，自营 ASN 挂在 `AS9009 (M247 Europe SRL)` 下，12 个机房里 7 个直接用 AS9009，其余走合作机房自己的 AS（AS396073 / AS14315 / AS35478 / AS39347）。每个机房页都公开了 **test IP**，**下单前请务必自己 ping / mtr 测一遍**，不要只看本文的结论。

| 机房 | 国家 | 类型 | 机房 / 运营商 | ASN | 上游 Transit | 互联 IX | Test IP |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [Silicon Valley](https://rarecloud.io/datacenters/silicon-valley-us/) | USA | VPS | OpenColo SC1 / OpenColo (Energy Group Networks) | AS396073 (Majestic Hosting Solutions) | NTT、GTT、Hurricane Electric、Cogent | — | `85.121.241.8` |
| [Phoenix](https://rarecloud.io/datacenters/phoenix-us/) | USA | VPS | Phoenix Datacenter / 1GServers | AS14315 (1GSERVERS LLC) | TATA Communications、NTT、Cogent | Ninja-IX Phoenix | `157.254.221.121` |
| [Dallas](https://rarecloud.io/datacenters/dallas-us/) | USA | VPS | Provision Data Services (SOURCE MCF) / Provision Data Services | AS396073 (Majestic Hosting Solutions) | Cogent、Zayo、EGIHosting | Equinix IX Dallas | `45.13.214.1` |
| [New York](https://rarecloud.io/datacenters/new-york-us/) | USA | VPS | Equinix NY2 / Equinix | AS9009 (M247 Europe SRL) | Arelion (Telia)、Cogent、NTT | DE-CIX New York、NYIIX | `72.14.147.2` |
| [London](https://rarecloud.io/datacenters/london-uk/) | United Kingdom | VPS | Digital Realty Cloud House (LHR19) / Digital Realty | AS9009 (M247 Europe SRL) | Arelion (Telia)、Cogent、GTT、TIS | LONAP、LINX | `85.121.48.2` |
| [The Hague](https://rarecloud.io/datacenters/the-hague-nl/) | Netherlands | VPS | Netrouting Data Facilities THG1 / Data Facilities DC (DFDC) | AS9009 (M247 Europe SRL) | Cogent | LSIX | `85.121.54.2` |
| [Frankfurt](https://rarecloud.io/datacenters/frankfurt-de/) | Germany | VPS | Telehouse 23Media / Telehouse (KDDI) | AS9009 (M247 Europe SRL) | Arelion (Telia)、Lumen (Level 3)、Cogent、GTT | DE-CIX、NL-IX、Equinix-IX | `85.121.52.2` |
| [Timisoara](https://rarecloud.io/datacenters/timisoara-ro/) | Romania | VPS | Bunea TELECOM DC / Bunea TELECOM SRL | AS35478 (Bunea TELECOM SRL) | Cogent、Arelion (Telia)、Orange Romania、Vodafone Romania、RETN | — | `45.13.38.2` |
| [Constanta](https://rarecloud.io/datacenters/constanta-ro/) | Romania | VPS | RareCloud DC Navodari / RareCloud / 07Internet | AS39347 (07Internet) | DIGI Romania | — | `85.122.120.20` |
| [Hong Kong](https://rarecloud.io/datacenters/hong-kong-hk/) | Hong Kong | VPS | Equinix HK2 / Equinix | AS9009 (M247 Europe SRL) | Lumen (Level 3)、Cogent、NTT、PCCW | Equinix、BBIX | `85.121.244.250` |
| [Tokyo](https://rarecloud.io/datacenters/tokyo-jp/) | Japan | VPS | Equinix TY8 / Equinix | AS9009 (M247 Europe SRL) | Cogent、NTT、PCCW | JPIX、BBIX | `85.121.50.2` |
| [Bucharest](https://rarecloud.io/datacenters/bucharest-ro/) | Romania | Cloud VM | M247 Bucharest, DC1 and DC2 / M247 | AS9009 (M247 Europe SRL) | Cogent、GTT、Arelion、Colt、TIS | Interlan、Balcan-IX、RoNIX、Netix | `85.120.226.190` |

| 机房 | 选它做什么 | 购买入口 |
| --- | --- | --- |
| [Silicon Valley](https://rarecloud.io/datacenters/silicon-valley-us/) | 美国业务落地；**稳定性评价最差**，仅在必需时选 | [选此机房下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) |
| [Phoenix](https://rarecloud.io/datacenters/phoenix-us/) | 美西备选，1GSERVERS 机房 | [选此机房下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) |
| [Dallas](https://rarecloud.io/datacenters/dallas-us/) | 美国中部业务 | [选此机房下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) |
| [New York](https://rarecloud.io/datacenters/new-york-us/) | 美东业务、面向北美东岸用户 | [选此机房下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) |
| [London](https://rarecloud.io/datacenters/london-uk/) | 欧洲用户评价最好的机房之一；被形容为「只有手动重启时才掉一下」 | [选此机房下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) |
| [The Hague](https://rarecloud.io/datacenters/the-hague-nl/) | 荷兰海牙，2025-12 迁入新机房、全部换 IP，部分用户称「联通快乐」 | [选此机房下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) |
| [Frankfurt](https://rarecloud.io/datacenters/frankfurt-de/) | **电信 / 联通**用户的首选：回程 4837 直连，CPU 也最好（Ryzen 7） | [选此机房下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) |
| [Timisoara](https://rarecloud.io/datacenters/timisoara-ro/) | 罗马尼亚本地机，多 homes 多家 Tier-1/2，回程同样走 4837 | [选此机房下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) |
| [Constanta](https://rarecloud.io/datacenters/constanta-ro/) | 干净未用过的本地 IPv4 段，**唯一不提供 IPv6** 的机房 | [选此机房下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) |
| [Hong Kong](https://rarecloud.io/datacenters/hong-kong-hk/) | 中国大陆**移动**用户；社区称「移动快乐鸡」，回程 CMI 直连 | [选此机房下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) |
| [Tokyo](https://rarecloud.io/datacenters/tokyo-jp/) | 调用美国 API 的业务；**电信用户不建议**，活动款之外丢包明显 | [选此机房下单 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) |
| [Bucharest](https://rarecloud.io/datacenters/bucharest-ro/) | **只在 Cloud VM 提供**，13 个规格都落在这里 | [选此机房下单 →](https://rarecloud.io/clients/aff.php?aff=1012) |

机房页与 test IP 来自官网 [https://rarecloud.io/datacenters/](https://rarecloud.io/datacenters/)；「选此机房下单」进入对应套餐的推广下单页，机房在结账时选择。

## 一、Linux KVM VPS —— 全站主力，8 个档位

### Linux KVM VPS —— 真 KVM、NVMe、11 个机房任选，全站最低 €1.56/月 `最低价` `可月付` `8 档` 

- **机房**：11 个机房任选（硅谷 / 凤凰城 / 达拉斯 / 纽约 / 伦敦 / 海牙 / 法兰克福 / 蒂米什瓦拉 / 康斯坦察 / 香港 / 东京），下单时选
- **虚拟化**：KVM 全虚拟化 —— 可加载内核模块、跑 Docker / WireGuard、自行更换内核或挂自己的 ISO
- **硬盘 / 流量**：全部 NVMe；每档均含 1 个 IPv4 + IPv6 子网（Advanced 为 /64，其余 /112）
- **系统**：Ubuntu、Debian、AlmaLinux、Rocky Linux、CentOS Stream 模板，可在面板一键重装
- **起价**：€1.56 / 月（Micro KVM：1 vCPU / 768MB RAM / 15GB NVMe / 1TB /month） [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=6)

#### 档位与价格

| 档位 | CPU | 内存 | 硬盘 | 流量 | IPv4 / IPv6 | 月付 | 季付 | 半年 | 年付 | 两年 | 三年 | 最低月均价 / 购买 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **Micro KVM** | 1 vCPU | 768MB RAM | 15GB NVMe | 1TB /month | 1x IPv4 & /112 IPv6 Subnet | — | — | — | [€1.62](https://rarecloud.io/clients/aff.php?aff=1012&pid=6) | [€1.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=6) | [€1.56](https://rarecloud.io/clients/aff.php?aff=1012&pid=6) | [**€1.56**](https://rarecloud.io/clients/aff.php?aff=1012&pid=6) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=6)　<small>（三年付，一次性付 €56.00）</small> |
| **Starter KVM** | 1 vCPU | 1GB RAM | 25GB NVMe | 3TB /month | 1x IPv4 & /112 IPv6 Subnet | — | — | — | [€2.46](https://rarecloud.io/clients/aff.php?aff=1012&pid=3) | [€2.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=3) | [€2.08](https://rarecloud.io/clients/aff.php?aff=1012&pid=3) | [**€2.08**](https://rarecloud.io/clients/aff.php?aff=1012&pid=3) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=3)　<small>（三年付，一次性付 €75.00）</small> |
| **Advanced KVM** | 1 vCPU | 2.5GB RAM | 45GB NVMe | 5TB /month | 1x IPv4 & /64 IPv6 Subnet | [€4.95](https://rarecloud.io/clients/aff.php?aff=1012&pid=11) | [€4.67](https://rarecloud.io/clients/aff.php?aff=1012&pid=11) | [€4.12](https://rarecloud.io/clients/aff.php?aff=1012&pid=11) | [€4.12](https://rarecloud.io/clients/aff.php?aff=1012&pid=11) | [€4.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=11) | [€3.89](https://rarecloud.io/clients/aff.php?aff=1012&pid=11) | [**€3.89**](https://rarecloud.io/clients/aff.php?aff=1012&pid=11) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)　<small>（三年付，一次性付 €140.00）</small> |
| **Core VPS** | 1 vCPU | 2GB RAM | 40GB NVMe | 3TB /month | 1x IPv4 & /112 IPv6 Subnet | [€5.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) | [€5.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) | [€3.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) | [€3.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) | [€3.33](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) | [€3.19](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) | [**€3.19**](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)　<small>（三年付，一次性付 €115.00）</small> |
| **Do It Yourself VPS** | 1–8 vCPU 自选 | 1–32 GB 自选 | 20–500 GB 自选 | 1–20 TB 自选 | 资源完全自定义，仅月付/年付 | [€7.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=16) | [€7.17](https://rarecloud.io/clients/aff.php?aff=1012&pid=16) | [€6.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=16) | [€6.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=16) | — | — | [**€6.25**](https://rarecloud.io/clients/aff.php?aff=1012&pid=16) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=16)　<small>（半年付，一次性付 €37.50）</small> |
| **Plus VPS** | 2 vCPU | 4GB RAM | 65GB NVMe | 5TB /month | 1x IPv4 & /112 IPv6 Subnet | [€9.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) | [€9.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) | [**€7.92**](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)　<small>（半年付，一次性付 €47.50）</small> |
| **Pro VPS** | 4 vCPU | 8GB RAM | 100GB NVMe | 7TB /month | 1x IPv4 & /112 IPv6 Subnet | [€19.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) | [€18.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) | [**€16.25**](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)　<small>（半年付，一次性付 €97.50）</small> |
| **Elite VPS** | 4 vCPU | 16GB RAM | 150GB NVMe | 10TB /month | 1x IPv4 & /112 IPv6 Subnet | [€34.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=15) | [€32.67](https://rarecloud.io/clients/aff.php?aff=1012&pid=15) | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=15) | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=15) | [€27.08](https://rarecloud.io/clients/aff.php?aff=1012&pid=15) | [€25.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=15) | [**€25.00**](https://rarecloud.io/clients/aff.php?aff=1012&pid=15) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)　<small>（三年付，一次性付 €900.00）</small> |

#### 产品特点与注意事项

这是 RareCloud 的基本盘，也是全部 19 个套餐里选择最多的一条线。8 个档位从 **768MB 内存的引流款**一路排到 16GB 内存，所有档位都是真 KVM + NVMe。

价格结构要单独说清楚：**月付最贵、三年付最便宜**；但最便宜的两档（Micro / Starter）**根本不提供月付**，必须一次付 1.5 年起步。另外 Plus / Pro 两档**两年付与三年付总价完全相同**——也就是说**锁三年并不会比锁两年更划算**，这两档最多锁两年。

- Micro KVM 的 **768MB 内存**是刻意做出来的引流款：能跑 WireGuard、静态页、轻量脚本，装完 Debian 后可用内存通常只剩 300MB 上下。**别拿它跑 Docker 或数据库。**
- Advanced KVM（1C/2.5G/45G）是这条线**唯一提供 /64 IPv6**的档位，其余都是 /112 子网；想要完整 IPv6 子网就选它。
- Do It Yourself 支持 vCPU 1→8、内存 1→32GB、硬盘 20→500GB、流量 1→20TB 全自选，但**只有月付到年付四个周期，没有两年付与三年付**。
- 硬件**按机房分化明显**：德国机房给 Ryzen 7 3700X / 5800X（Geekbench 5 单核 982–1100），其他机房多为 Xeon E5-2683 v4 / E5-2690 v2（GB5 约 400–548）。买德国机等于顺带拿到更好的 CPU。

#### 适用运营商

- **中国联通**：★★★
- **中国电信**：★★☆
- **中国移动**：★★★
- **教育网**：—

依据强度：实测　|　11 个机房全部可选。**移动优先选香港**（回程 CMI 直连，社区称「移动快乐鸡」）；**电信 / 联通优先选德国**（法兰克福 / 蒂米什瓦拉，回程联通 4837 直连，延迟约 180–260ms）；**电信不要选香港和东京**，回程被判定绕路（英国→欧洲→香港→美国）且丢包。荷兰海牙迁站后被部分用户称为「联通快乐」。美国四城延迟高且稳定性评价最差，只适合放纯海外业务。

> 「Rarecloud €8.3/年 德国三网直连 上海这联通电信好香。。25三年还能买」
>
> —— 《Rarecloud €8.3/年 德国三网直连》, 2025-02-02　[《Rarecloud €8.3/年 德国三网直连》, 2025-02-02](https://www.nodeseek.com/post-242618-1)

> 「综合来看，硬盘读写都差不多，德国机房硬件较好，CPU 的 GB5 分数上 1000，线路也是直连的，延迟也不错」
>
> —— 《【测评】Rarecloud 各区域机房测评》, 2024-12-30　[《【测评】Rarecloud 各区域机房测评》, 2024-12-30](https://www.nodeseek.com/post-213762-1)

> 「优点：处理器分数较高；网络直连中国；电信、联通延迟低于 200ms……缺点：CPU 和内存性能差一些；需要免税账号」
>
> —— 《【三德机对比】Rarecloud vs Delux vs Netcup》, 2024-10-29　[《【三德机对比】Rarecloud vs Delux vs Netcup》, 2024-10-29](https://www.nodeseek.com/post-176102-1)

> 「rarecloud 这家的机器现在只剩罗马尼亚一个位置？……rarecloud 的机器相对来说欧洲节点要稳定一些，美国节点稳定性很差，经常关机或者丢包率高到没边了」
>
> —— 《rarecloud 失联》, 2026-10-03　[《rarecloud 失联》, 2026-10-03](https://www.nodeseek.com/post-958377-1)

**适合谁：**预算极低、能接受「年付当赌博」的人；大陆移动用户想要一台便宜的香港机；需要真 KVM 但对 CPU 性能要求不高的轻量服务。

**不适合：**需要放生产业务的人（社区「宕机 / 失联 / 工单不回」的帖子密度很高）；中国电信用户买香港 / 东京机；指望靠 14 天退款兜底的人。

**本线全部档位的推广购买入口：**[Micro KVM €1.56/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=6)　[Starter KVM €2.08/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=3)　[Advanced KVM €3.89/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)　[Core VPS €3.19/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)　[Do It Yourself VPS €6.25/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=16)　[Plus VPS €7.92/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)　[Pro VPS €16.25/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)　[Elite VPS €25.00/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)

**购买入口**：[查看 Linux KVM VPS 全部配置与价格 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=6)

## 二、Windows RDP VPS —— 3 个档位

### Windows VPS —— 团队远程桌面共用的常开 Windows 机器 `需自购授权` `3 档` 

- **机房**：同样 11 个机房任选，与 Linux 档位共用机房与网络
- **系统**：Windows Server 模板，RDP 远程桌面，完全管理员权限
- **硬盘 / 流量**：全部 NVMe；每档均含 1 个 IPv4 + IPv6 子网
- **授权**：模板自带 180 天评估期；正式商用须自行向微软或授权经销商购买许可证（可自带激活）
- **起价**：€12.92 / 月（Win 4G：2 vCPUs / 4GB RAM / 60GB NVMe / 4TB /month） [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=7)

#### 档位与价格

| 档位 | CPU | 内存 | 硬盘 | 流量 | IPv4 / IPv6 | 月付 | 季付 | 半年 | 年付 | 两年 | 三年 | 最低月均价 / 购买 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **Win 4G** | 2 vCPUs | 4GB RAM | 60GB NVMe | 4TB /month | 1x IPv4 & /112 IPv6 Subnet | [€15.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=7) | — | — | [€12.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=7) | [€12.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=7) | [€12.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=7) | [**€12.92**](https://rarecloud.io/clients/aff.php?aff=1012&pid=7) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=7)　<small>（年付，一次性付 €155.00）</small> |
| **Win 8G** | 4 vCPUs | 8GB RAM | 120GB NVMe | 6TB /month | 1x IPv4 & /112 IPv6 Subnet | [€29.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=17) | — | — | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=17) | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=17) | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=17) | [**€24.58**](https://rarecloud.io/clients/aff.php?aff=1012&pid=17) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=17)　<small>（年付，一次性付 €295.00）</small> |
| **Win 12G** | 4 vCPUs | 12GB RAM | 160GB NVMe | 10TB /month | 1x IPv4 & /112 IPv6 Subnet | [€34.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=18) | — | — | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=18) | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=18) | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=18) | [**€28.75**](https://rarecloud.io/clients/aff.php?aff=1012&pid=18) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=18)　<small>（年付，一次性付 €345.00）</small> |

#### 产品特点与注意事项

三个档位分别是 Win 4G（2C/4G/60G/4TB）、Win 8G（4C/8G/120G/6TB）、Win 12G（4C/12G/160G/10TB）。定位很明确：一台 7×24 小时开着、团队用远程桌面共享的 Windows 机器——跑没有 Linux 版的桌面软件、.NET / IIS / SQL Server，或者给工作室当常驻节点。

★ **授权必须自己解决**：RareCloud 只提供 Windows Server 模板，官方模板自带 **180 天评估期**；正式商用要自行向微软或授权经销商购买许可证，已有 Windows Server 授权的可以自带激活。这一点在下单前一定要算进成本。

- Win 系列**只提供月付 / 年付 / 两年付 / 三年付四档**（没有季付与半年付），而且**年付、两年付、三年付同价**，锁长周期没有任何折扣——锁两年最划算。
- 社区对 Windows 档位的测评样本很少，选之前建议先用 Linux 档或 Cloud VM 试手。

#### 适用运营商

- **中国联通**：★★☆
- **中国电信**：★★☆
- **中国移动**：★★☆
- **教育网**：—

依据强度：实测　|　与 Linux 档位共用同一套机房，选点建议相同：移动优先香港，电信 / 联通优先德国。远程桌面对延迟比网页更敏感，建议离办公地点或常用出口近一些。

> 「One server can be the always-on machine a whole team shares, for example accountants working in shifts on the same desktop software」（官方产品页）
>
> —— RareCloud Windows VPS 产品页 FAQ　[RareCloud Windows VPS 产品页 FAQ](https://rarecloud.io/windows-vps/)

**适合谁：**需要一台常开 Windows 机器的团队（会计轮班、跑特定桌面软件、内部工具）。

**不适合：**个人开发者（Linux 档位便宜一半以上）；已经在用 Windows 实体机或云桌面的人。

**本线全部档位的推广购买入口：**[Win 4G €12.92/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=7)　[Win 8G €24.58/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=17)　[Win 12G €28.75/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=18)

**购买入口**：[查看 Windows RDP VPS 全部配置与价格 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=7)

## 三、n8n 自动化 VPS —— 2 个档位

### n8n VPS —— 预装 n8n 与 HTTPS，开箱即用，年付折合 €4.00/月 `年付最划算` `无执行次数限制` 

- **机房**：11 个机房任选
- **预装内容**：n8n + Nginx 反向代理 + Let's Encrypt 证书 + UFW 防火墙（只开 22 / 80 / 443）
- **上线方式**：SSH 后执行 `bash /root/setup-domain.sh yourdomain.com` 绑定域名并自动签发证书
- **执行限制**：无次数限制；Starter 用 SQLite，Pro 用 PostgreSQL 16 + Redis 7 + 2 个 worker
- **起价**：€4.00 / 月（N8N Starter：2 vCPU / 4GB RAM / 65GB NVMe / 5TB /month） [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=36)

#### 档位与价格

| 档位 | CPU | 内存 | 硬盘 | 流量 | IPv4 / IPv6 | 月付 | 季付 | 半年 | 年付 | 两年 | 三年 | 最低月均价 / 购买 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **N8N Starter** | 2 vCPU | 4GB RAM | 65GB NVMe | 5TB /month | 预装 n8n（SQLite）+ Nginx + SSL | [€9.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=36) | — | — | [€4.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=36) | — | — | [**€4.00**](https://rarecloud.io/clients/aff.php?aff=1012&pid=36) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=36)　<small>（年付，一次性付 €48.00）</small> |
| **N8N PRO** | 4 vCPU | 8GB RAM | 100GB NVMe | 7TB /month | 预装 n8n（Docker + PG16 + Redis） | [€19.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=37) | — | — | [€5.69](https://rarecloud.io/clients/aff.php?aff=1012&pid=37) | — | — | [**€5.69**](https://rarecloud.io/clients/aff.php?aff=1012&pid=37) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=37)　<small>（年付，一次性付 €68.25）</small> |

#### 产品特点与注意事项

n8n 是自建工作流自动化的热门开源工具，官方云版按执行次数收费。RareCloud 的做法是**把 n8n、Nginx 反代、证书和防火墙全部预装好**，你只需要 SSH 进去跑一条 `setup-domain.sh` 就能上线，不用碰 Docker、反向代理或证书。

★ 这条线的**年付折扣是全站最猛的**：Starter 月付 €9.50、年付总价 €48（折合 **€4.00/月**），Pro 月付 €19.50、年付 €68.25（折合 €5.69/月）。官方明确写「无执行次数限制」——只要 CPU 和内存扛得住就跑多少。

- Starter 是 npm 原生安装 + SQLite 嵌入式数据库，适合小项目；Pro 是 Docker 容器化，PostgreSQL 16 与 Redis **不对公网暴露**，只允许 n8n 内部访问。
- 注意 n8n Starter（pid 36）与 OpenClaw Server（pid 49）**价格完全一样**，Pro 与 Desktop 同理——这两条线在后台共用同一套计费配置。
- n8n 官方强调不要把编辑器直接暴露到公网。RareCloud 的方案是 Nginx + HTTPS + 只开三端口，但**仍建议自己再套一层访问控制**（IP 白名单或 Basic Auth）。

#### 适用运营商

- **中国联通**：★★★
- **中国电信**：★★★
- **中国移动**：★★★
- **教育网**：—

依据强度：实测　|　这条线是「应用服务器」场景，客户端是你的工作流，不是访客，线路本身要求不高。如果工作流要调用欧洲的 API（OpenAI / Anthropic 等），选**德国或荷兰**机房更顺。

> 「n8n, PostgreSQL 和 Redis run as separate containers, so an update or a rollback is one image away」（官方产品页）
>
> —— RareCloud n8n VPS 产品页　[RareCloud n8n VPS 产品页](https://rarecloud.io/n8n-vps/)

**适合谁：**想低成本自建工作流自动化，替代按执行次数计费的 n8n 云版；不想折腾 Docker、反代与证书的人。

**不适合：**需要多节点集群或高可用部署的人；工作流计算量很大、Starter 的 CPU 扛不住的场景。

**本线全部档位的推广购买入口：**[N8N Starter €4.00/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=36)　[N8N PRO €5.69/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=37)

**购买入口**：[查看 n8n 自动化 VPS 全部配置与价格 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=36)

## 四、OpenClaw AI 助手 VPS —— 2 个档位

### OpenClaw VPS —— 把 AI 助手放在自己机器上，年付折合 €4.00/月 `数据留在自己机器` `8 层加固` 

- **机房**：11 个机房任选
- **预装内容**：OpenClaw（最新版）+ headless Chrome；nftables、fail2ban、AppArmor profile
- **安全策略**：仪表盘默认只监听 localhost，需经 SSH 隧道访问；自动安全更新已开启
- **接入渠道**：Telegram / WhatsApp / Discord / Slack / Signal；模型用你自己的 Anthropic 或 OpenAI key
- **起价**：€4.00 / 月（OpenClaw Server：2 vCPU / 4GB RAM / 65GB NVMe / 5TB /month） [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=49)

#### 档位与价格

| 档位 | CPU | 内存 | 硬盘 | 流量 | IPv4 / IPv6 | 月付 | 季付 | 半年 | 年付 | 两年 | 三年 | 最低月均价 / 购买 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **OpenClaw Server** | 2 vCPU | 4GB RAM | 65GB NVMe | 5TB /month | 预装 OpenClaw（headless Chrome） | [€9.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=49) | — | — | [€4.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=49) | — | — | [**€4.00**](https://rarecloud.io/clients/aff.php?aff=1012&pid=49) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=49)　<small>（年付，一次性付 €48.00）</small> |
| **OpenClaw Desktop** | 4 vCPU | 8GB RAM | 100GB NVMe | 7TB /month | 预装 OpenClaw + XFCE 图形桌面 | [€19.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=50) | — | — | [€5.69](https://rarecloud.io/clients/aff.php?aff=1012&pid=50) | — | — | [**€5.69**](https://rarecloud.io/clients/aff.php?aff=1012&pid=50) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=50)　<small>（年付，一次性付 €68.25）</small> |

#### 产品特点与注意事项

OpenClaw 是一个开源自托管 AI 助手。RareCloud 把它连同浏览器一起预装好，并按官方说法做了 **8 层安全加固**：nftables 防火墙、fail2ban、AppArmor profile、仪表盘**只监听 localhost**、自动安全更新。

Server 档从 **2 vCPU / 4GB / 65GB NVMe / 5TB** 起步，Desktop 档从 **4 vCPU / 8GB / 100GB NVMe / 7TB** 起步，后者多一套 **XFCE 图形桌面 + 非 headless 的 Chrome / Firefox**，可以从控制面板用 VNC 看 AI 实时点网页、填表单。两条线都是**可自定义配置**的。

- 对隐私敏感的用法来说这是最大卖点：**对话记录和 API key 都留在你自己的服务器上**，RareCloud 不经手。
- 「让 AI 操作浏览器」本身风险不小，建议用 Desktop 档时保留 AppArmor 隔离，并给不同的机器人分配不同的服务器。
- ⚠️ **官网自身数据打架**：WHMCS 产品描述里 Desktop 写 2C/8G/60G，而官网产品卡写 4C/8G/100GB。本文采用**官网产品卡**的数据，下单前建议以控制台实际配置为准。

#### 适用运营商

- **中国联通**：★★★
- **中国电信**：★★★
- **中国移动**：★★★
- **教育网**：—

依据强度：实测　|　与 API 供应商的连通性优先于大陆延迟。若调用 OpenAI / Anthropic 等美国接口，选美西机房响应更快；若调用欧洲接口，选德国 / 荷兰。

> 「Your data stays on your server. We never see your API keys or conversations」（官方产品页）
>
> —— RareCloud OpenClaw VPS 产品页　[RareCloud OpenClaw VPS 产品页](https://rarecloud.io/openclaw-vps/)

**适合谁：**想把 AI 助手的对话记录和密钥留在自己机器上的人；想低成本多开一个 AI 助手实例的人。

**不适合：**对「AI 自动操作浏览器」没有安全意识的人（建议先在低权限容器里试）；需要官方托管与 SLA 兜底的企业场景。

**本线全部档位的推广购买入口：**[OpenClaw Server €4.00/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=49)　[OpenClaw Desktop €5.69/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=50)

**购买入口**：[查看 OpenClaw AI 助手 VPS 全部配置与价格 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=49)

## 五、Web 虚拟主机 —— 4 个档位

### Web 虚拟主机 —— cPanel 一键装 WordPress，最低 €2.22/月 `含免费域名` `每日备份` 

- **面板**：cPanel，一键安装 WordPress（Softaculous）、免费 SSL、每日备份、独立 IP
- **免费迁移**：从旧主机迁移网站、数据库与邮箱，官方免费代做
- **年限**：不适用——虚拟主机没有年付款概念，按月 / 周期付
- **注意**：★ Enterprise 档的两年付与三年付与 Business 档同价，疑似定价未同步，买前先开工单确认
- **起价**：€2.22 / 月（Website Hosting：共享 / 共享 / 10GB NVMe / 不限流量） [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=51)

#### 档位与价格

| 档位 | CPU | 内存 | 硬盘 | 流量 | IPv4 / IPv6 | 月付 | 季付 | 半年 | 年付 | 两年 | 三年 | 最低月均价 / 购买 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **Website Hosting** | 共享 | 共享 | 10GB NVMe | 不限流量 | 10 个邮箱 · 送 .com 域名 · 99.9% uptime | — | — | — | [€2.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=51) | [€2.29](https://rarecloud.io/clients/aff.php?aff=1012&pid=51) | [€2.22](https://rarecloud.io/clients/aff.php?aff=1012&pid=51) | [**€2.22**](https://rarecloud.io/clients/aff.php?aff=1012&pid=51) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=51)　<small>（三年付，一次性付 €80.00）</small> |
| **StartUp** | 1.5 核 | 2GB RAM | 50GB NVMe | 不限流量 | 1 个网站 · 独立 IP · 送 SSL | [€9.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=21) | — | — | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=21) | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=21) | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=21) | [**€7.92**](https://rarecloud.io/clients/aff.php?aff=1012&pid=21) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=21)　<small>（年付，一次性付 €95.00）</small> |
| **Business** | 3 核 | 4GB RAM | 100GB NVMe | 不限流量 | 不限站点 · 独立 IP · 送 SSL + 域名 | [€19.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=22) | — | — | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=22) | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=22) | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=22) | [**€16.25**](https://rarecloud.io/clients/aff.php?aff=1012&pid=22) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=22)　<small>（年付，一次性付 €195.00）</small> |
| **Enterprise** | 6 核 | 8GB RAM | 不限 NVMe | 不限流量 | 不限站点 · 独立 IP · 送 SSL + 域名 | [€39.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=23) | — | — | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=23) | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=23) | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=23) | [**€16.25**](https://rarecloud.io/clients/aff.php?aff=1012&pid=23) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=23)　<small>（两年付，一次性付 €390.00）</small> |

#### 产品特点与注意事项

给不想碰服务器的人准备的。四个档位从 **Website Hosting（年付 €30，折合 €2.22/月）**起，再到 StartUp / Business / Enterprise 三档不限量站点方案：不限流量、免费 SSL、每日备份、独立 IP，Business 及以上送域名注册。

★ 这条线有个**明显的定价异常值得避坑**：Enterprise 档月付 €39.50、年付 €295，但**两年付 €390、三年付 €585，和低一档的 Business 完全相同**。也就是说 Enterprise 锁长周期不但没有溢价，还比它自己月付便宜一大截——这多半是后台配置没同步，买之前建议先开工单问清楚。

- Website Hosting（pid 51）**只有年付 / 两年付 / 三年付，没有月付**，配置是 10GB NVMe、不限流量、10 个邮箱、送 .com 域名、99.9% uptime 保证。
- StartUp / Business / Enterprise 三档都能建不限量站点，差别在核数、内存与硬盘（50GB → 100GB → 不限）。

#### 适用运营商

- **中国联通**：★★★
- **中国电信**：★★★
- **中国移动**：★★★
- **教育网**：—

依据强度：实测　|　虚拟主机的客户端是网站访客，浏览器访问，线路敏感度低，三网都可用。社区里建站反馈普遍是「够用」，德国机房被多次提到「真香」。

> 「Already hosted somewhere else? We move your site, databases and mailboxes for free」（官方产品页）
>
> —— RareCloud Web Hosting 产品页　[RareCloud Web Hosting 产品页](https://rarecloud.io/web-hosting/)

**适合谁：**只需要一个 WordPress 或静态站、不想碰服务器运维的人；需要免费迁移与每日备份的人。

**不适合：**需要 SSH / 自定义 PHP 扩展 / 邮件服务器的人（虚拟主机不给 root）；需要自己装 n8n、Docker 之类应用的人（那是 VPS 线）。

**本线全部档位的推广购买入口：**[Website Hosting €2.22/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=51)　[StartUp €7.92/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=21)　[Business €16.25/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=22)　[Enterprise €16.25/月](https://rarecloud.io/clients/aff.php?aff=1012&pid=23)

**购买入口**：[查看 Web 虚拟主机 全部配置与价格 →](https://rarecloud.io/clients/aff.php?aff=1012&pid=51)

## 六、Cloud VM 与云附加件（13 规格）

### Cloud VM —— 布加勒斯特，13 个规格按小时计费、月价封顶 `按小时`

- **机房**：仅布加勒斯特（M247 Bucharest, DC1 / DC2），不提供 VPS 档位
- **计费**：按小时出账，当月费用封顶在月价；先用量后付费，月末开票
- **含流量**：1 TB – 12 TB 随规格递增
- **含公网 IPv4**：每台都自带，不额外收费
- **起价**：[€3.99 / 月封顶](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012)（S-1 · €0.0055/小时）

#### 13 个规格

| 规格 | 家族 | vCPU | 内存 | NVMe | 含流量 | 小时价 / 购买 | 月价封顶 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| **S-1** | Cost-Optimized | 1 共享 | 2 GB | 25 GB | 1 TB | [€0.0055/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€3.99](https://rarecloud.io/clients/aff.php?aff=1012) |
| **S-2** | Cost-Optimized | 2 共享 | 4 GB | 50 GB | 2 TB | [€0.0096/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€6.99](https://rarecloud.io/clients/aff.php?aff=1012) |
| **S-4** | Cost-Optimized | 4 共享 | 8 GB | 80 GB | 4 TB | [€0.0178/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€12.99](https://rarecloud.io/clients/aff.php?aff=1012) |
| **G-1** | General Purpose | 1 共享 | 4 GB | 60 GB | 4 TB | [€0.0109/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€7.99](https://rarecloud.io/clients/aff.php?aff=1012) |
| **G-2** | General Purpose（推荐） | 2 共享 | 8 GB | 100 GB | 6 TB | [€0.0205/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€14.99](https://rarecloud.io/clients/aff.php?aff=1012) |
| **G-4** | General Purpose | 4 共享 | 16 GB | 160 GB | 8 TB | [€0.0383/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€27.99](https://rarecloud.io/clients/aff.php?aff=1012) |
| **G-8** | General Purpose | 8 共享 | 32 GB | 240 GB | 12 TB | [€0.0726/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€52.99](https://rarecloud.io/clients/aff.php?aff=1012) |
| **C-2** | CPU-Optimized | 2 专用 | 4 GB | 80 GB | 6 TB | [€0.0274/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€19.99](https://rarecloud.io/clients/aff.php?aff=1012) |
| **C-4** | CPU-Optimized | 4 专用 | 8 GB | 120 GB | 8 TB | [€0.0520/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€37.99](https://rarecloud.io/clients/aff.php?aff=1012) |
| **C-8** | CPU-Optimized | 8 专用 | 16 GB | 200 GB | 12 TB | [€0.1000/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€72.99](https://rarecloud.io/clients/aff.php?aff=1012) |
| **M-2** | Memory-Optimized | 2 共享 | 16 GB | 80 GB | 6 TB | [€0.0616/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€44.99](https://rarecloud.io/clients/aff.php?aff=1012) |
| **M-4** | Memory-Optimized | 4 共享 | 32 GB | 160 GB | 8 TB | [€0.1164/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€84.99](https://rarecloud.io/clients/aff.php?aff=1012) |
| **M-8** | Memory-Optimized | 8 共享 | 64 GB | 320 GB | 12 TB | [€0.2192/h](https://rarecloud.io/clients/aff.php?aff=1012) [部署](https://rarecloud.io/clients/aff.php?aff=1012) | [€159.99](https://rarecloud.io/clients/aff.php?aff=1012) |

#### 计费规则

Cloud VM 和前面的 VPS 是**两套完全不同的计费体系**：只在**布加勒斯特**一个机房，**按小时计费、当月费用封顶在月价**。13 个规格分四个家族：Cost-Optimized（S）、General Purpose（G）、CPU-Optimized（C）、Memory-Optimized（M）。

官网自己给了横向对比：**G-2**（2 共享 vCPU / 8GB / 100GB NVMe / 6TB 流量）€14.99/月，而 Hetzner CPX32 要 €35.99、DigitalOcean Basic Premium AMD 要 $42、Vultr 4/8 要 $40（标价对比，均不含 IPv4 附加费的差异已在官网表中标注）。

每个 Cloud VM 都自带**公网 IPv4、NVMe 存储、云防火墙、私网**，并且支持随时改配置而**不换 IP**。Cloud 资源是**先用量后付费**：月末出账，账上有余额 / 赠金会在出账时自动抵扣；账单低于 €5 顺延到下期。

- **资源只要存在就计费，跟开关机无关**，删掉才停止计费。
- 欠费超过 7 天，会在**账单国家当地时间 09:00** 关机（关机不等于删除）；再过 14 天连同数据**永久删除**，删除前至少提前 24 小时邮件通知。
- 欠费期间不能创建新的 Cloud 资源。托管 K8s 集群休眠时 worker 节点会被移除并停止计费，但**卷仍继续计费**。

可用系统：Ubuntu 24.04 LTS、Ubuntu 22.04 LTS、Debian 12、Rocky Linux 9（也可从自己的快照创建）

#### 按需付费的附加服务

| 服务 | 价格 | 购买入口 |
| --- | --- | --- |
| 快照 Snapshot | €0.05 / GB / 月，每台最多 5 个，单个最低 €0.25 | [部署时添加 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| 块存储 Block Storage | €0.05 / GB / 月，单卷最大 2 TB，可分离后带数据迁移到别的机器 | [部署时添加 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| 保留 IP Reserved IP | €2 / 月 | [部署时添加 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| 负载均衡 Load Balancer | €9 / 月（含公网 IP），L4 + 健康检查 | [部署时添加 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| 对象存储 Object Storage | €10 / 月含 1 TB（S3 兼容，aws-cli / rclone / 各家 S3 SDK 都能用） | [部署时添加 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| Managed Kubernetes | 控制面免费，worker 从 €7.99 / 月起 | [部署时添加 →](https://rarecloud.io/clients/aff.php?aff=1012) |

**购买入口**：[前往控制台部署 Cloud VM →](https://rarecloud.io/clients/aff.php?aff=1012)

## 全部 19 个套餐与推广入口

一张表列全所有套餐，点击任意价格或「购买」都会带推广参数进入该套餐的下单页。机房在结账时选择。

| 产品线 | 套餐 | CPU | 内存 | 硬盘 | 流量 | 可用周期 | 最低月均价 / 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Linux KVM VPS | Starter KVM | 1 vCPU | 1GB RAM | 25GB NVMe | 3TB /month | 年付 / 两年 / 三年 | [€2.08](https://rarecloud.io/clients/aff.php?aff=1012&pid=3) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=3) <small>（三年付，一次性付 €75.00）</small> |
| Linux KVM VPS | Micro KVM | 1 vCPU | 768MB RAM | 15GB NVMe | 1TB /month | 年付 / 两年 / 三年 | [€1.56](https://rarecloud.io/clients/aff.php?aff=1012&pid=6) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=6) <small>（三年付，一次性付 €56.00）</small> |
| Linux KVM VPS | Advanced KVM | 1 vCPU | 2.5GB RAM | 45GB NVMe | 5TB /month | 月付 / 季付 / 半年 / 年付 / 两年 / 三年 | [€3.89](https://rarecloud.io/clients/aff.php?aff=1012&pid=11) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=11) <small>（三年付，一次性付 €140.00）</small> |
| Linux KVM VPS | Core VPS | 1 vCPU | 2GB RAM | 40GB NVMe | 3TB /month | 月付 / 季付 / 半年 / 年付 / 两年 / 三年 | [€3.19](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=12) <small>（三年付，一次性付 €115.00）</small> |
| Linux KVM VPS | Plus VPS | 2 vCPU | 4GB RAM | 65GB NVMe | 5TB /month | 月付 / 季付 / 半年 / 年付 / 两年 / 三年 | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=13) <small>（半年付，一次性付 €47.50）</small> |
| Linux KVM VPS | Pro VPS | 4 vCPU | 8GB RAM | 100GB NVMe | 7TB /month | 月付 / 季付 / 半年 / 年付 / 两年 / 三年 | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=14) <small>（半年付，一次性付 €97.50）</small> |
| Linux KVM VPS | Elite VPS | 4 vCPU | 16GB RAM | 150GB NVMe | 10TB /month | 月付 / 季付 / 半年 / 年付 / 两年 / 三年 | [€25.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=15) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=15) <small>（三年付，一次性付 €900.00）</small> |
| Linux KVM VPS | Do It Yourself VPS | 1–8 vCPU 自选 | 1–32 GB 自选 | 20–500 GB 自选 | 1–20 TB 自选 | 月付 / 季付 / 半年 / 年付 | [€6.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=16) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=16) <small>（半年付，一次性付 €37.50）</small> |
| Windows RDP VPS | Win 4G | 2 vCPUs | 4GB RAM | 60GB NVMe | 4TB /month | 月付 / 年付 / 两年 / 三年 | [€12.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=7) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=7) <small>（年付，一次性付 €155.00）</small> |
| Windows RDP VPS | Win 8G | 4 vCPUs | 8GB RAM | 120GB NVMe | 6TB /month | 月付 / 年付 / 两年 / 三年 | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=17) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=17) <small>（年付，一次性付 €295.00）</small> |
| Windows RDP VPS | Win 12G | 4 vCPUs | 12GB RAM | 160GB NVMe | 10TB /month | 月付 / 年付 / 两年 / 三年 | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=18) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=18) <small>（年付，一次性付 €345.00）</small> |
| 应用预装 VPS | N8N Starter | 2 vCPU | 4GB RAM | 65GB NVMe | 5TB /month | 月付 / 年付 | [€4.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=36) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=36) <small>（年付，一次性付 €48.00）</small> |
| 应用预装 VPS | N8N PRO | 4 vCPU | 8GB RAM | 100GB NVMe | 7TB /month | 月付 / 年付 | [€5.69](https://rarecloud.io/clients/aff.php?aff=1012&pid=37) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=37) <small>（年付，一次性付 €68.25）</small> |
| 应用预装 VPS | OpenClaw Server | 2 vCPU | 4GB RAM | 65GB NVMe | 5TB /month | 月付 / 年付 | [€4.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=49) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=49) <small>（年付，一次性付 €48.00）</small> |
| 应用预装 VPS | OpenClaw Desktop | 4 vCPU | 8GB RAM | 100GB NVMe | 7TB /month | 月付 / 年付 | [€5.69](https://rarecloud.io/clients/aff.php?aff=1012&pid=50) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=50) <small>（年付，一次性付 €68.25）</small> |
| Web 虚拟主机 | StartUp | 1.5 核 | 2GB RAM | 50GB NVMe | 不限流量 | 月付 / 年付 / 两年 / 三年 | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=21) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=21) <small>（年付，一次性付 €95.00）</small> |
| Web 虚拟主机 | Business | 3 核 | 4GB RAM | 100GB NVMe | 不限流量 | 月付 / 年付 / 两年 / 三年 | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=22) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=22) <small>（年付，一次性付 €195.00）</small> |
| Web 虚拟主机 | Enterprise | 6 核 | 8GB RAM | 不限 NVMe | 不限流量 | 月付 / 年付 / 两年 / 三年 | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=23) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=23) <small>（两年付，一次性付 €390.00）</small> |
| Web 虚拟主机 | Website Hosting | 共享 | 共享 | 10GB NVMe | 不限流量 | 年付 / 两年 / 三年 | [€2.22](https://rarecloud.io/clients/aff.php?aff=1012&pid=51) [购买](https://rarecloud.io/clients/aff.php?aff=1012&pid=51) <small>（三年付，一次性付 €80.00）</small> |

## 社区口碑：被认可与被吐槽

下面每一条都来自 NodeSeek 帖子的正文或评论，附原帖链接，可逐条复核。
**价格优势与风险评价同时存在**，建议两边都看完。

### 被认可的地方

| 结论 | 依据 | 出处 |
| --- | --- | --- |
| **价格是真的低** | 三年付 €25 的 1C/1G/25G/3T，在当年是全网最低梯队；黑五活动款甚至到过 €9.75/年。 | 2025-02-02　[《Rarecloud €8.3/年 德国三网直连》](https://www.nodeseek.com/post-242618-1) |
| **德国机房硬件确实更好** | 德国机给 Ryzen 7 3700X / 5800X，Geekbench 5 单核 982、SysBench 单线程 1906；社区测评明确写「德国机房硬件较好，CPU 的 GB5 分数上 1000，线路也是直连的」。 | 2025-05-18　[《【评测】RareCloud 德国 1H2.5G 45G SSD 闪购服务器测评》](https://www.nodeseek.com/post-342100-1) |
| **移动用户能拿到真香香港机** | 香港回程 CMI 直连，有用户从日本迁到香港后表示「用得很爽」，社区通称「移动快乐鸡」。 | 2025-12-20　[《【测评】Rarecloud 新机房测评（香港）移动快乐机》](https://www.nodeseek.com/post-541236-1) |
| **平时其实挺稳** | 「探针一直很稳定，基本上只有机房升级才有问题。用了两年倒没发现什么问题，工单响应挺及时」——另一位老用户自述开了两台机器、用了一年多才发现被多开了一台并被删掉。 | 2026-05-15　[《咨询一下各位老外商家 rarecloud 的灵车程度》](https://www.nodeseek.com/post-732070-1) |
| **欧盟主体、可开 VAT 发票** | 运营方是罗马尼亚 RARE MOOD AGENCY SRL（Tax ID 45192771），支持信用卡 / 借记卡、PayPal、支付宝、加密货币与银行转账。 | 2026-10-14　[RareCloud 服务条款](https://rarecloud.io/tos/) |

### 被吐槽的地方

| 问题 | 社区原话 / 依据 | 出处 |
| --- | --- | --- |
| **退款极难，14 天政策形同虚设** | 「12 月 1 日买的 vps，后面申请工单退款，到现在快一个月了都没有退款成功」；有人被反复以「上报高层」为由拖延两个月。社区共识是「**一定要用 PayPal 付**，支付宝没办法」。 | 2025-12-26　[《避坑垃圾商家 rarecloud》](https://www.nodeseek.com/post-559090-1) |
| **稳定性波动明显** | 2025-06「IP 所有地方都不通」持续一整天；2026-08、2026-10 连续出现「又挂了」「失联」帖；社区结论是「欧洲节点要稳定一些，美国节点稳定性很差，经常关机或者丢包率高到没边了」。 | 2026-10-03　[《rarecloud 失联》](https://www.nodeseek.com/post-958377-1) |
| **续费已经涨过一轮** | 2026-09 官方通知续费涨价：25 欧三年付涨到 37.5 欧三年付；有用户反馈「我的从大概 25o 一年变成 100o 一年」。邮件明确 Pro VPS (VM9) 自 **2028-01-24** 起为 $113.25/年（当前标价 $226.49，保留 50% 折扣）。 | 2026-09-07　[《【慢讯】rarecloud 续费涨价了》](https://www.nodeseek.com/post-916089-1) |
| **充值赠金是明显的坑** | 「25 欧元以下，充多少，送多少……续费时，最多且只能续一个周期，如果之前就续费过，现在连第一个周期都没结束，那根本没法用赠金去续费」，而且赠金**只有 60 天有效期**。社区把「50o 翻 3 倍」直接当作跑路前的高风险信号。 | 2026-09-05　[《讲讲 RareCloud 充值 3 倍 / 4 倍的套路》](https://www.nodeseek.com/post-888388-1) |
| **强制迁移会整段换 IP** | 2025-12 荷兰节点整体迁到海牙新机房，退役 45.129.13.0/24、45.148.11.0/24、45.142.192.0/24，迁移后**全部换新 IP**；硅谷节点同样退役多个 /24。条款也写明 IP 不可携带、不可转让。 | 2025-12-14　[《RareCloud 将要迁移 荷兰VPS位置，换IP》](https://www.nodeseek.com/post-530431-1) |
| **老款可能被降配** | 有用户翻出一台三年前的老机重测：「单核 5800x 被干成了 9254」「内存也降了，只有 1.5G 了」——商家在基础设施迁移后把老机器换到了新硬件上。 | 2026-06-14　[《[老机新测] Rarecloud 翻出来一个老鸡》](https://www.nodeseek.com/post-763050-1) |
| **IP 质量与流媒体全线拉胯** | 「不要指望解锁，广播 IP，Gemini 给你飞罗马尼亚，或者送美送中，chatgpt 直接显示你是 VPN」。 | 2026-05-15　[《咨询一下各位老外商家 rarecloud 的灵车程度》](https://www.nodeseek.com/post-732070-1) |
| **商家自己不做备份** | 条款写明：除非服务协议另有说明，RareCloud **不做任何客户数据备份**，硬件故障、误操作导致的数据丢失概不负责。 | 2026-10-14　[RareCloud 服务条款](https://rarecloud.io/tos/) |

## 常见问题

### RareCloud 是什么来头？

运营方是**罗马尼亚**的 RARE MOOD AGENCY SRL（Tax ID 45192771，VAT RO45192771，Reg. No. J13/3713/2021），背后是罗马尼亚持牌电信运营商 **M247**（AS9009），12 个数据中心里有 7 个直接挂在 M247 的 AS9009 下。它不是空壳新号，但确实是**近两年在社区里争议很大的低价商家**——「价格真香」和「随时可能跑路」两种评价同时存在。建议按年付玩具 / 副业机器的定位买。

### 最便宜多少钱？真能买到吗？

**€1.56/月**——Micro KVM（1 vCPU / 768MB / 15GB NVMe / 1TB 流量），**一次付三年 €56**。注意 Micro 和 Starter **没有月付**，最低一次性付 1.5 年；768MB 内存装完系统基本就满了。

### 可以按月付吗？

Linux KVM 里的 Advanced / Core / DIY / Plus / Pro / Elite 与全部 Windows、n8n、OpenClaw 档位都可以月付；**只有 Micro KVM、Starter KVM、Website Hosting 三档没有月付**。Cloud VM 全部按小时计费、封顶月价。

### 哪些套餐锁长周期不划算？

**Plus VPS、Pro VPS、Win 4G / 8G / 12G 的两年付与三年付总价完全相同**，锁三年没有任何额外折扣，这几档最多锁两年。Enterprise 虚拟主机也有类似异常（两年付 / 三年付与 Business 同价），买前建议开工单确认。

### 中国大陆用户选哪个机房？

**移动选香港**（回程 CMI 直连，社区称「移动快乐鸡」）；**电信 / 联通选德国**（法兰克福 / 蒂米什瓦拉，回程联通 4837 直连，延迟约 180–260ms）；**电信不要选香港和东京**，回程绕路、丢包明显。美国四城只适合纯海外业务。

### 怎么验证线路好不好？

每个数据中心页面都直接给了 test IP，例如法兰克福 `85.121.52.2`、伦敦 `85.121.48.2`、海牙 `85.121.54.2`、东京 `85.121.50.2`、香港 `85.121.244.250`。下单前先 `ping` 和 `mtr` 测一遍再付钱。

### 支持支付宝吗？

支持。官方条款列出的支付方式是信用卡 / 借记卡、PayPal、**支付宝**、加密货币和银行转账。但社区一致提醒：**想退款就用 PayPal 付**，支付宝单几乎没成功退款的。

### 有备份吗？

没有。条款明确写了除非另有说明，RareCloud 不为客户数据做备份，硬件故障、误操作导致的数据丢失概不负责。Cloud VM 有快照服务（€0.05/GB/月，每台最多 5 个），KVM VPS 档位得自己解决备份。

### 退款政策是怎样的？

条款写的是 **14 天退款**（需满足「使用量极少」等条件），超出后按 as-is 处理，除非 30 天内换机或转余额。但社区反馈是：工单经常只回复「已上报高层」，有人退款拖了两个月，最后靠 **PayPal 争议**秒退。

### IP 会被换掉吗？

会。历史上荷兰节点从原机房迁到海牙时**整段 IP 全换**（退役 45.129.13.0/24、45.148.11.0/24、45.142.192.0/24），硅谷节点也退役过多个 /24。条款明确 IP 不可迁移、不可转让。建议用第三方托管 DNS，别把解析挂在会变动的 IP 上。

### 能解锁流媒体 / 用 ChatGPT 吗？

IP 基本是广播段。有用户直接反馈「Gemini 定位飞到罗马尼亚，ChatGPT 直接判定为 VPN」。如果你的用途依赖干净的住宅 / 机房 IP，请另找专门商家。

### Micro KVM 的 768MB 内存能干什么？

够跑 WireGuard、反向代理、静态站、轻量脚本和监控 agent。**不够**跑 Docker（哪怕一个容器）、数据库、Java 项目或任何带编译的工具链。装完 Debian 后可用内存通常只剩 300MB 上下。如果只是想要「一台便宜的常在线机器」，它很合适；想跑服务请至少上 Core VPS（2GB）。

### Cloud VM 和 KVM VPS 有什么区别？该选哪个？

KVM VPS 是**预付固定周期**（月付到三年付），11 个机房任选，适合长期持有；Cloud VM 是**按小时后付费、月价封顶**，只在布加勒斯特，但支持随时改配置而不换 IP、自带云防火墙与私网，适合弹性负载和短期测试。

## 选购注意事项与风险提示

> **下单前务必确认这几点。**这些不是「劝退」，而是让你**用对预期**——
> RareCloud 的低价是真的，它的不确定性也是真的，两件事同时成立。
>
> - **先开机，别囤赠金。**充值赠金**只有 60 天有效期**，且「续费时最多且只能续一个周期」。手上的 VPS 越早开、周期排得越靠前，赠金越用得上；反过来先充值再慢慢开机，赠金大概率白瞎。
> - **锁多久合适：默认 1 年，最多 2 年。**年付比月付便宜 15%–17%，三年付再便宜一档；但 2026-09 已经涨过一轮，条款也没有长期锁价承诺。**Plus / Pro / Win 系列的两年付与三年付同价，锁三年纯属多担风险。**
> - **迁移风险要自己消化。**历史上已发生多轮大规模迁移（荷兰 → 海牙、硅谷退役 IP 段、老机换硬件）。条款明确「IP 是服务的一部分，不可携带、不可转让，商家改号会尽力避免中断」。**DNS 记录别写死 IP**，有条件就用 Cloudflare 之类的托管解析。
> - **付款方式决定了你的退路。**官方支持信用卡 / 借据卡、PayPal、支付宝、加密货币、银行转账。**社区的一致建议是优先用 PayPal**——支付宝订单几乎没有成功退款的先例。
> - **价格不含 VAT。**官网价格全部是**不含税**价。欧盟客户若无有效 VAT ID，会被加收 **19% 罗马尼亚增值税**；中国大陆用户在结账前务必确认最终应付金额。
> - **别把它当生产主力。**99.9% uptime 的 SLA 写在条款里（低于阈值可按 downtime 的 10%/1% 申请退月费，需开工单），但 SLA 赔付和退款一样要看客服脸色。生产业务建议**年付一台 + 自己做快照 + 准备兜底方案**。
> - **商家已发过「涨价预告 + 给半月原价窗口」的邮件。**有用户按 2026-06 的邮件在涨价前续了费，随后续费价仍然上调；另有用户在赠金还没用完时就续了两次，结果赠金彻底花不出去。**不要把促销邮件当成锁价承诺。**
> - **14 天退款不是兜底。**条款写的是 14 天（需满足「使用量极少」等条件），超出后按 as-is 处理。但社区执行情况是：工单经常只回「已上报高层」，有人拖了两个月，最后靠 **PayPal 争议**秒退。

如果这些风险你都不能接受，建议看同价位更稳的商家；如果能接受，那 RareCloud 的性价比确实是第一梯队的。

## 数据来源与引用

产品、价格与机房数据来自 RareCloud 官网；线路与口碑结论来自 NodeSeek 社区，
按主题整理了以下帖子作为依据，可逐条复核：

### NodeSeek 帖子

1. [测评] [【测评】Rarecloud各区域机房测评（罗马尼亚、凤凰城、硅谷、阿姆斯特丹、德国）](https://www.nodeseek.com/post-213762-1)　—　weyony，2024-12-30，10 条评论
2. [测评] [【评测】RareCloud 德国 1H2.5G 45G SSD 闪购服务器 测评](https://www.nodeseek.com/post-342100-1)　—　WuZihan，2025-05-18，9 条评论
3. [测评] [【三德机对比】Rarecloud vs Delux vs Netcup（10欧/年）/Rarecloud 优惠码RARE45可以用了，限时优惠！](https://www.nodeseek.com/post-176102-1)　—　weyony，2024-10-29，9 条评论
4. [情报] [Rarecloud €8.3/年  德国三网直连 上海这联通电信好香。。25三年还能买](https://www.nodeseek.com/post-242618-1)　—　jack9225，2025-02-02，10 条评论
5. [测评] [【测评】Rarecloud新机房测评（香港）移动快乐机](https://www.nodeseek.com/post-541236-1)　—　weyony，2025-12-20，11 条评论
6. [测评] [rarecloud hk 晚高峰北方移动测评](https://www.nodeseek.com/post-814658-1)　—　nzg，2026-07-10，6 条评论
7. [测评] [Rarecloud 9.9欧 日本东京 测试留档](https://www.nodeseek.com/post-491166-1)　—　luopojunzi，2025-10-30，10 条评论
8. [日常] [rarecloud 日本区，在黑五之后频繁掉线](https://www.nodeseek.com/post-532002-1)　—　ageg，2025-12-05，7 条评论
9. [情报] [讲讲 RareCloud 充值 3 倍 / 4 倍的套路](https://www.nodeseek.com/post-888388-1)　—　AhFei，2026-09-05，10 条评论
10. [日常] [rarecloud是想跑路了？ 推出的充值翻倍活动是否有点离谱了，50o翻3倍](https://www.nodeseek.com/post-805485-1)　—　kki，2026-07-22，10 条评论
11. [日常] [rarecloud正式通知续费涨价了](https://www.nodeseek.com/post-912278-1)　—　东道主，2026-09-05，10 条评论
12. [日常] [【慢讯】rarecloud续费涨价了](https://www.nodeseek.com/post-916089-1)　—　hihaboy，2026-09-07，8 条评论
13. [情报] [rarecloud失联](https://www.nodeseek.com/post-958377-1)　—　firebet，2026-10-03，10 条评论
14. [日常] [rarecloud又挂了](https://www.nodeseek.com/post-879170-1)　—　nolog，2026-08-21，10 条评论
15. [日常] [rarecloud机房出问题了？IP所有地方都不通](https://www.nodeseek.com/post-364185-1)　—　娃md-150，2025-06-18，10 条评论
16. [日常] [rarecloud退款真牛逼！](https://www.nodeseek.com/post-503828-1)　—　noders，2025-11-19，10 条评论
17. [日常] [避坑垃圾商家rarecloud](https://www.nodeseek.com/post-559090-1)　—　rainman，2025-12-26，8 条评论
18. [日常] [rarecloud，避雷，已申请退款](https://www.nodeseek.com/post-562682-1)　—　Sharon210，2026-01-17，10 条评论
19. [日常] [rarecloud这家服务很差](https://www.nodeseek.com/post-500487-1)　—　tergarsam，2025-11-19，10 条评论
20. [测评] [rarecloud退款battle了两个月，给重开了一台](https://www.nodeseek.com/post-511128-1)　—　bahua，2025-11-21，10 条评论
21. [日常] [警惕rarecloud](https://www.nodeseek.com/post-903678-1)　—　，2026-10-14，3 条评论
22. [情报] [RareCloud 将要迁移 荷兰VPS位置，换IP](https://www.nodeseek.com/post-530431-1)　—　pretty，2025-12-14，10 条评论
23. [情报] [RareCloud 又又要开始迁移了](https://www.nodeseek.com/post-550633-1)　—　pretty，2025-12-20，10 条评论
24. [测评] [[老机新测] Rarecloud 翻出来一个老鸡1c2g 3年25o，才发现半年前被商家迁移了机房](https://www.nodeseek.com/post-763050-1)　—　Codec，2026-06-14，10 条评论
25. [日常] [咨询一下各位老外商家rarecloud的灵车程度](https://www.nodeseek.com/post-732070-1)　—　hahaaa，2026-05-15，10 条评论
26. [情报] [【快讯】RareCloud.io活动](https://www.nodeseek.com/post-390934-1)　—　清见琉璃，2025-07-12，6 条评论
27. [日常] [RareCloud到底怎么样？](https://www.nodeseek.com/post-793846-1)　—　peterbosnia，2026-07-07，10 条评论

### 官网页面

- **官网**：[RareCloud Linux VPS 产品与价格页](https://rarecloud.io/kvm-vps/) — <https://rarecloud.io/kvm-vps/>
- **官网**：[RareCloud Cloud VM 页（13 个规格与横向对比）](https://rarecloud.io/cloud-vm/) — <https://rarecloud.io/cloud-vm/>
- **官网**：[RareCloud 数据中心总览（12 机房）](https://rarecloud.io/datacenters/) — <https://rarecloud.io/datacenters/>
- **官网**：[RareCloud 服务条款（SLA / 退款 / 备份 / IP / VAT）](https://rarecloud.io/tos/) — <https://rarecloud.io/tos/>
- **官网**：[RareCloud 联盟计划（15% 持续佣金）](https://rarecloud.io/affiliates/) — <https://rarecloud.io/affiliates/>
- **官网**：[定价数据源：WHMCS 导出 JSON（last_updated 2026-10-14 04:00:01）](https://rarecloud.io/data/whmcs-pricing.json) — <https://rarecloud.io/data/whmcs-pricing.json>

采集方式：本机 Chrome 登录态 + CDP。NodeSeek 搜索「rarecloud」共抓取 417 条结果，
其中 202 篇抓取了正文与评论（共 1761 条评论）。
产品与价格为抓取时点快照，以官网实时信息为准。

---

本文为第三方产品整理，与 RareCloud 官方无隶属关系。文中购买链接含推广参数（aff=1012），不影响你的购买价格。价格与库存随时可能变动，请以 [RareCloud 官网](https://rarecloud.io/kvm-vps/) 为准。
