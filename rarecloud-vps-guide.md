# RareCloud VPS 全产品线选购指南

> 数据快照：2026-10-14。RareCloud（rarecloud.io）是罗马尼亚 M247（AS9009）旗下的低价 VPS 品牌，
> 最低 **€1.56/月**起。本文拆解官网 **19 个可下单套餐**与 **12 个数据中心**。
> 全文购买链接均带推广标识 `aff=1012`，通过链接下单不会多收你的钱。

## 先看结论：7 条速览

- **谁在运营** — RareCloud 是**罗马尼亚**公司 RARE MOOD AGENCY SRL（Tax ID 45192771，VAT RO45192771）旗下的 VPS / 云品牌，背后就是持牌电信运营商 **M247**（AS9009）。NodeSeek 社区里也有人指出它「以前叫 VPSforVPN」——同一条 M247 网络，换了层皮做零售。
- **卖什么** — 四条产品线共 **19 个可下单套餐**：Linux KVM VPS（8 档）、Windows RDP VPS（3 档）、n8n 自动化 VPS（2 档）、OpenClaw AI 助手 VPS（2 档），外加 4 档 Web 虚拟主机与布加勒斯特的 Cloud VM。
- **最低价** — **€1.56/月**（Micro KVM，768MB 内存，1TB 流量，*一次付三年*）。注意：Micro / Starter / Website Hosting **没有月付档**，最低一次性付 1.5 年。
- **机房** — **12 个数据中心**：11 个 VPS 机房（硅谷、凤凰城、达拉斯、纽约、伦敦、海牙、法兰克福、蒂米什瓦拉、康斯坦察、香港、东京）+ 1 个 Cloud VM 机房（布加勒斯特）。每个机房官网都给了 **test IP**，可以自己 ping / mtr 验证。
- **谁适合买** — ① 预算极低、能接受「年付当赌博」的人（年付 €9.75～€30 的活动款是它真正的价值所在）；② 大陆**移动**用户想要一台便宜的香港机；③ 想低成本跑 n8n / OpenClaw 这类预装应用的人。
- **谁不适合** — ① 需要放**生产业务**的人——2025–2026 社区里「宕机 / 失联 / 工单不回」的帖子密度很高；② 指望**退款**兜底的人——14 天退款写在条款里，实际执行极难，社区共识是「用 PayPal 付款，走 PayPal 争议」；③ 中国**电信**用户——香港 / 日本机房回程绕路，延迟高、丢包重。
- **★ 必须先知道** — 2026-09 起官方**通知续费涨价**；2025-12 荷兰节点强制迁移、退役多个 IP 段并更换全部 IP；充值赠金**只有 60 天有效期**且续费一次只能用掉一个周期。本文所有价格都是抓取时点快照，长期持有务必按「随时可能涨价、随时可能换 IP」来规划。

## 全部 19 个套餐与真实月均价

表内数字是**按付款周期摊薄的每月底价**（不是一次性总价），点任意价格即通过推广链接进入下单页。「—」表示该套餐不提供这个周期。

### Linux KVM VPS

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | IP | 月付 | 季付 | 半年付 | 年付 | 两年付 | 三年付 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| **Starter KVM** | 1 vCPU | 1GB RAM | 25GB NVMe | 3TB /month | 1x IPv4 & /112 IPv6 Subnet | — | — | — | [€2.46](https://rarecloud.io/clients/aff.php?aff=1012&pid=3)<br>*年付 · 付 €29.50* | [€2.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=3)<br>*两年付 · 付 €54.00* | [€2.08](https://rarecloud.io/clients/aff.php?aff=1012&pid=3)<br>*三年付 · 付 €75.00* |
| **Micro KVM** | 1 vCPU | 768MB RAM | 15GB NVMe | 1TB /month | 1x IPv4 & /112 IPv6 Subnet | — | — | — | [€1.62](https://rarecloud.io/clients/aff.php?aff=1012&pid=6)<br>*年付 · 付 €19.50* | [€1.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=6)<br>*两年付 · 付 €38.00* | [€1.56](https://rarecloud.io/clients/aff.php?aff=1012&pid=6)<br>*三年付 · 付 €56.00* |
| **Advanced KVM** | 1 vCPU | 2.5GB RAM | 45GB NVMe | 5TB /month | 1x IPv4 & /64 IPv6 Subnet | [€4.95](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)<br>*月付 · 付 €4.95* | [€4.67](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)<br>*季付 · 付 €14.00* | [€4.12](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)<br>*半年付 · 付 €24.75* | [€4.12](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)<br>*年付 · 付 €49.50* | [€4.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)<br>*两年付 · 付 €96.00* | [€3.89](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)<br>*三年付 · 付 €140.00* |
| **Core VPS** | 1 vCPU | 2GB RAM | 40GB NVMe | 3TB /month | 1x IPv4 & /112 IPv6 Subnet | [€5.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)<br>*月付 · 付 €5.50* | [€5.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)<br>*季付 · 付 €15.00* | [€3.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)<br>*半年付 · 付 €22.50* | [€3.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)<br>*年付 · 付 €45.00* | [€3.33](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)<br>*两年付 · 付 €80.00* | [€3.19](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)<br>*三年付 · 付 €115.00* |
| **Plus VPS** | 2 vCPU | 4GB RAM | 65GB NVMe | 5TB /month | 1x IPv4 & /112 IPv6 Subnet | [€9.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)<br>*月付 · 付 €9.50* | [€9.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)<br>*季付 · 付 €27.00* | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)<br>*半年付 · 付 €47.50* | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)<br>*年付 · 付 €95.00* | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)<br>*两年付 · 付 €190.00* | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)<br>*三年付 · 付 €285.00* |
| **Pro VPS** | 4 vCPU | 8GB RAM | 100GB NVMe | 7TB /month | 1x IPv4 & /112 IPv6 Subnet | [€19.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)<br>*月付 · 付 €19.50* | [€18.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)<br>*季付 · 付 €55.50* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)<br>*半年付 · 付 €97.50* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)<br>*年付 · 付 €195.00* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)<br>*两年付 · 付 €390.00* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)<br>*三年付 · 付 €585.00* |
| **Elite VPS** | 4 vCPU | 16GB RAM | 150GB NVMe | 10TB /month | 1x IPv4 & /112 IPv6 Subnet | [€34.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)<br>*月付 · 付 €34.50* | [€32.67](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)<br>*季付 · 付 €98.00* | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)<br>*半年付 · 付 €172.50* | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)<br>*年付 · 付 €345.00* | [€27.08](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)<br>*两年付 · 付 €650.00* | [€25.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)<br>*三年付 · 付 €900.00* |
| **Do It Yourself VPS** | 1 → 8 vCPU（自选） | 1 → 32 GB（自选） | 20 → 500 GB（自选） | 1 → 20 TB（自选） | 资源完全自定义 | [€7.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=16)<br>*月付 · 付 €7.50* | [€7.17](https://rarecloud.io/clients/aff.php?aff=1012&pid=16)<br>*季付 · 付 €21.50* | [€6.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=16)<br>*半年付 · 付 €37.50* | [€6.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=16)<br>*年付 · 付 €75.00* | — | — |

### Windows RDP VPS

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | IP | 月付 | 季付 | 半年付 | 年付 | 两年付 | 三年付 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| **Win 4G** | 2 vCPUs | 4GB RAM | 60GB NVMe | 4TB /month | 1x IPv4 & /112 IPv6 Subnet | [€15.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=7)<br>*月付 · 付 €15.50* | — | — | [€12.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=7)<br>*年付 · 付 €155.00* | [€12.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=7)<br>*两年付 · 付 €310.00* | [€12.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=7)<br>*三年付 · 付 €465.00* |
| **Win 8G** | 4 vCPUs | 8GB RAM | 120GB NVMe | 6TB /month | 1x IPv4 & /112 IPv6 Subnet | [€29.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=17)<br>*月付 · 付 €29.50* | — | — | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=17)<br>*年付 · 付 €295.00* | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=17)<br>*两年付 · 付 €590.00* | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=17)<br>*三年付 · 付 €885.00* |
| **Win 12G** | 4 vCPUs | 12GB RAM | 160GB NVMe | 10TB /month | 1x IPv4 & /112 IPv6 Subnet | [€34.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=18)<br>*月付 · 付 €34.50* | — | — | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=18)<br>*年付 · 付 €345.00* | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=18)<br>*两年付 · 付 €690.00* | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=18)<br>*三年付 · 付 €1035.00* |

### 应用预装 VPS（n8n / OpenClaw）

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | IP | 月付 | 季付 | 半年付 | 年付 | 两年付 | 三年付 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| **N8N Starter** | 2 vCPU | 4GB RAM | 65GB NVMe | 5TB /month | 预装 n8n（SQLite）+ Nginx + SSL | [€9.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=36)<br>*月付 · 付 €9.50* | — | — | [€4.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=36)<br>*年付 · 付 €48.00* | — | — |
| **N8N PRO** | 4 vCPU | 8GB RAM | 100GB NVMe | 7TB /month | 预装 n8n（Docker + PG16 + Redis） | [€19.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=37)<br>*月付 · 付 €19.50* | — | — | [€5.69](https://rarecloud.io/clients/aff.php?aff=1012&pid=37)<br>*年付 · 付 €68.25* | — | — |
| **OpenClaw Server** | 2 vCPU | 4GB RAM | 65GB NVMe | 5TB /month | 预装 OpenClaw（headless Chrome） | [€9.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=49)<br>*月付 · 付 €9.50* | — | — | [€4.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=49)<br>*年付 · 付 €48.00* | — | — |
| **OpenClaw Desktop** | 4 vCPU | 8GB RAM | 100GB NVMe | 7TB /month | 预装 OpenClaw + XFCE 图形桌面 | [€19.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=50)<br>*月付 · 付 €19.50* | — | — | [€5.69](https://rarecloud.io/clients/aff.php?aff=1012&pid=50)<br>*年付 · 付 €68.25* | — | — |

### Web 虚拟主机

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | IP | 月付 | 季付 | 半年付 | 年付 | 两年付 | 三年付 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| **StartUp** | 1.5 核 | 2GB RAM | 50GB NVMe | 不限流量 | 1 个网站 · 独立 IP · 送 SSL | [€9.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=21)<br>*月付 · 付 €9.50* | — | — | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=21)<br>*年付 · 付 €95.00* | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=21)<br>*两年付 · 付 €190.00* | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=21)<br>*三年付 · 付 €285.00* |
| **Business** | 3 核 | 4GB RAM | 100GB NVMe | 不限流量 | 不限站点 · 独立 IP · 送 SSL + 域名 | [€19.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=22)<br>*月付 · 付 €19.50* | — | — | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=22)<br>*年付 · 付 €195.00* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=22)<br>*两年付 · 付 €390.00* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=22)<br>*三年付 · 付 €585.00* |
| **Enterprise** | 6 核 | 8GB RAM | 不限 NVMe | 不限流量 | 不限站点 · 独立 IP · 送 SSL + 域名 | [€39.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=23)<br>*月付 · 付 €39.50* | — | — | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=23)<br>*年付 · 付 €295.00* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=23)<br>*两年付 · 付 €390.00* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=23)<br>*三年付 · 付 €585.00* |
| **Website Hosting** | 共享 | 共享 | 10GB NVMe | 不限流量 | 10 个邮箱 · 送 .com 域名 · 99.9% uptime | — | — | — | [€2.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=51)<br>*年付 · 付 €30.00* | [€2.29](https://rarecloud.io/clients/aff.php?aff=1012&pid=51)<br>*两年付 · 付 €55.00* | [€2.22](https://rarecloud.io/clients/aff.php?aff=1012&pid=51)<br>*三年付 · 付 €80.00* |

> **三条必须记住的价格规则：**

> 1. **Micro KVM、Starter KVM、Website Hosting 没有月付**，最低一次性付 1.5 年；

> 2. **Plus / Pro / Elite / Win 系列的两年付与三年付同价**，锁三年没有任何额外折扣；

> 3. 官网所有价格**不含 VAT**，欧盟客户若无 VAT ID 会加收 19% 罗马尼亚增值税。

## 12 个数据中心：机房、ASN、上游与 test IP

RareCloud 是 Tier III 机房 + Tier-1 出口的批发型网络，自营 ASN 挂在 `AS9009 (M247 Europe SRL)` 下。每个机房都有公开的 test IP，**下单前请务必自己 ping / mtr 测一遍**。

| 机房 | 机房 / 运营商 | ASN | 上游 Transit | 互联 IX | Test IP |
|---|---|---|---|---|---|
| [Silicon Valley](https://rarecloud.io/datacenters/silicon-valley-us/)（USA · VPS） | OpenColo SC1 / OpenColo (Energy Group Networks) | `AS396073 (Majestic Hosting Solutions)` | NTT、GTT、Hurricane Electric、Cogent | — | `85.121.241.8` |
| [Phoenix](https://rarecloud.io/datacenters/phoenix-us/)（USA · VPS） | Phoenix Datacenter / 1GServers | `AS14315 (1GSERVERS LLC)` | TATA Communications、NTT、Cogent | Ninja-IX Phoenix | `157.254.221.121` |
| [Dallas](https://rarecloud.io/datacenters/dallas-us/)（USA · VPS） | Provision Data Services (SOURCE MCF) / Provision Data Services | `AS396073 (Majestic Hosting Solutions)` | Cogent、Zayo、EGIHosting | Equinix IX Dallas | `45.13.214.1` |
| [New York](https://rarecloud.io/datacenters/new-york-us/)（USA · VPS） | Equinix NY2 / Equinix | `AS9009 (M247 Europe SRL)` | Arelion (Telia)、Cogent、NTT | DE-CIX New York、NYIIX | `72.14.147.2` |
| [London](https://rarecloud.io/datacenters/london-uk/)（United Kingdom · VPS） | Digital Realty Cloud House (LHR19) / Digital Realty | `AS9009 (M247 Europe SRL)` | Arelion (Telia)、Cogent、GTT、TIS | LONAP、LINX | `85.121.48.2` |
| [The Hague](https://rarecloud.io/datacenters/the-hague-nl/)（Netherlands · VPS） | Netrouting Data Facilities THG1 / Data Facilities DC (DFDC) | `AS9009 (M247 Europe SRL)` | Cogent | LSIX | `85.121.54.2` |
| [Frankfurt](https://rarecloud.io/datacenters/frankfurt-de/)（Germany · VPS） | Telehouse 23Media / Telehouse (KDDI) | `AS9009 (M247 Europe SRL)` | Arelion (Telia)、Lumen (Level 3)、Cogent、GTT | DE-CIX、NL-IX、Equinix-IX | `85.121.52.2` |
| [Timisoara](https://rarecloud.io/datacenters/timisoara-ro/)（Romania · VPS） | Bunea TELECOM DC / Bunea TELECOM SRL | `AS35478 (Bunea TELECOM SRL)` | Cogent、Arelion (Telia)、Orange Romania、Vodafone Romania、RETN | — | `45.13.38.2` |
| [Constanta](https://rarecloud.io/datacenters/constanta-ro/)（Romania · VPS） | RareCloud DC Navodari / RareCloud / 07Internet | `AS39347 (07Internet)` | DIGI Romania | — | `85.122.120.20` |
| [Hong Kong](https://rarecloud.io/datacenters/hong-kong-hk/)（Hong Kong · VPS） | Equinix HK2 / Equinix | `AS9009 (M247 Europe SRL)` | Lumen (Level 3)、Cogent、NTT、PCCW | Equinix、BBIX | `85.121.244.250` |
| [Tokyo](https://rarecloud.io/datacenters/tokyo-jp/)（Japan · VPS） | Equinix TY8 / Equinix | `AS9009 (M247 Europe SRL)` | Cogent、NTT、PCCW | JPIX、BBIX | `85.121.50.2` |
| [Bucharest](https://rarecloud.io/datacenters/bucharest-ro/)（Romania · Cloud VM） | M247 Bucharest, DC1 and DC2 / M247 | `AS9009 (M247 Europe SRL)` | Cogent、GTT、Arelion、Colt、TIS | Interlan、Balcan-IX、RoNIX、Netix | `85.120.226.190` |

布加勒斯特（Bucharest）是唯一的 **Cloud VM** 机房，其余 11 个只卖 KVM / Windows / 预装应用 VPS。康斯坦察（Constanta）**不提供 IPv6**。

## 大陆三网 × 机房适配矩阵

| 机房 | 中国电信 | 中国联通 | 中国移动 | 结论 |
|---|---|---|---|---|
| 德国 / 罗马尼亚（欧洲） | 可用但非优化线路；回程 4837 / CMI / CMIN2，延迟普遍 180–260ms | 可用。回程走联通 4837，测评中属「普通线路」，延迟低于 200ms | 相对友好，回程 CMI，部分地区命中 CMIN2 精品线路 | ★ 三个大洲里对大陆最稳的一档，也是社区公认硬件最好的机房（Ryzen 7 3700X/5800X） |
| 中国香港 | 不推荐。回程被判定绕路（英国→欧洲→香港→美国→北京），丢包且延迟高 | 不推荐，同样绕路，延迟与丢包都偏高 | ★ 全站对大陆移动最友好的机房，社区通称「移动快乐鸡」 | 只推给移动用户；且部分服务（ChatGPT / Gemini）在香港段不可用 |
| 日本东京 | 不推荐，社区多次提到电信方向绕路 | 一般 | 部分活动期表现好，活动结束后丢包明显；另有帖子反映日本区频繁掉线 | 除非特价（黑五 ¥9.75/年 那类），否则不如香港 |
| 美国（硅谷 / 凤凰城 / 达拉斯 / 纽约） | 延迟高（约 150–200ms 以上），且稳定性评价最差 | 延迟高 | 延迟高 | 社区反馈「美区稳定性很差，经常关机或丢包率高到没边」，只适合放纯海外业务 |
| 英国 / 荷兰 / 罗马尼亚其他机房 | 可用，无大陆优化 | 荷兰（海牙）被用户称为「联通快乐」 | 可用 | 2025-12 荷兰节点整体迁到海牙新机房，IP 段全部更换；英国节点评价「非常好，只有手动重启时才掉一下」 |

> **一句话选型：**移动用户优先**香港**，电信 / 联通优先**德国（法兰克福 / 蒂米什瓦拉）**，纯海外业务再考虑**美国**，**电信用户不要选香港和东京**（回程绕路、丢包）。

## 逐条产品线详解

### 一、Linux KVM VPS —— 全站主力，8 个档位

**Linux KVM VPS：真 KVM、NVMe、11 个机房任选**

这是 RareCloud 的基本盘。所有 Linux 档位都是**KVM 全虚拟化**，可以加载内核模块、跑 Docker / WireGuard、自己换内核，也能从面板重装 Ubuntu、Debian、AlmaLinux、Rocky Linux、CentOS Stream，或直接挂自己的 ISO。

价格结构值得单独说：**月付最贵、三年付最便宜**，但最便宜的两档（Micro / Starter）**根本不提供月付**，必须一次付 1.5 年起步。另外 Plus / Pro / Win 系列的「两年付」和「三年付」总价完全相同，也就是说**锁三年并不会比锁两年更划算**——这两档锁两年就好。

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | IP | 月付 | 季付 | 半年付 | 年付 | 两年付 | 三年付 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| **Starter KVM** | 1 vCPU | 1GB RAM | 25GB NVMe | 3TB /month | 1x IPv4 & /112 IPv6 Subnet | — | — | — | [€2.46](https://rarecloud.io/clients/aff.php?aff=1012&pid=3)<br>*年付 · 付 €29.50* | [€2.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=3)<br>*两年付 · 付 €54.00* | [€2.08](https://rarecloud.io/clients/aff.php?aff=1012&pid=3)<br>*三年付 · 付 €75.00* |
| **Micro KVM** | 1 vCPU | 768MB RAM | 15GB NVMe | 1TB /month | 1x IPv4 & /112 IPv6 Subnet | — | — | — | [€1.62](https://rarecloud.io/clients/aff.php?aff=1012&pid=6)<br>*年付 · 付 €19.50* | [€1.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=6)<br>*两年付 · 付 €38.00* | [€1.56](https://rarecloud.io/clients/aff.php?aff=1012&pid=6)<br>*三年付 · 付 €56.00* |
| **Advanced KVM** | 1 vCPU | 2.5GB RAM | 45GB NVMe | 5TB /month | 1x IPv4 & /64 IPv6 Subnet | [€4.95](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)<br>*月付 · 付 €4.95* | [€4.67](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)<br>*季付 · 付 €14.00* | [€4.12](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)<br>*半年付 · 付 €24.75* | [€4.12](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)<br>*年付 · 付 €49.50* | [€4.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)<br>*两年付 · 付 €96.00* | [€3.89](https://rarecloud.io/clients/aff.php?aff=1012&pid=11)<br>*三年付 · 付 €140.00* |
| **Core VPS** | 1 vCPU | 2GB RAM | 40GB NVMe | 3TB /month | 1x IPv4 & /112 IPv6 Subnet | [€5.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)<br>*月付 · 付 €5.50* | [€5.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)<br>*季付 · 付 €15.00* | [€3.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)<br>*半年付 · 付 €22.50* | [€3.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)<br>*年付 · 付 €45.00* | [€3.33](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)<br>*两年付 · 付 €80.00* | [€3.19](https://rarecloud.io/clients/aff.php?aff=1012&pid=12)<br>*三年付 · 付 €115.00* |
| **Plus VPS** | 2 vCPU | 4GB RAM | 65GB NVMe | 5TB /month | 1x IPv4 & /112 IPv6 Subnet | [€9.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)<br>*月付 · 付 €9.50* | [€9.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)<br>*季付 · 付 €27.00* | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)<br>*半年付 · 付 €47.50* | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)<br>*年付 · 付 €95.00* | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)<br>*两年付 · 付 €190.00* | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=13)<br>*三年付 · 付 €285.00* |
| **Pro VPS** | 4 vCPU | 8GB RAM | 100GB NVMe | 7TB /month | 1x IPv4 & /112 IPv6 Subnet | [€19.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)<br>*月付 · 付 €19.50* | [€18.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)<br>*季付 · 付 €55.50* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)<br>*半年付 · 付 €97.50* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)<br>*年付 · 付 €195.00* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)<br>*两年付 · 付 €390.00* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=14)<br>*三年付 · 付 €585.00* |
| **Elite VPS** | 4 vCPU | 16GB RAM | 150GB NVMe | 10TB /month | 1x IPv4 & /112 IPv6 Subnet | [€34.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)<br>*月付 · 付 €34.50* | [€32.67](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)<br>*季付 · 付 €98.00* | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)<br>*半年付 · 付 €172.50* | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)<br>*年付 · 付 €345.00* | [€27.08](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)<br>*两年付 · 付 €650.00* | [€25.00](https://rarecloud.io/clients/aff.php?aff=1012&pid=15)<br>*三年付 · 付 €900.00* |
| **Do It Yourself VPS** | 1 → 8 vCPU（自选） | 1 → 32 GB（自选） | 20 → 500 GB（自选） | 1 → 20 TB（自选） | 资源完全自定义 | [€7.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=16)<br>*月付 · 付 €7.50* | [€7.17](https://rarecloud.io/clients/aff.php?aff=1012&pid=16)<br>*季付 · 付 €21.50* | [€6.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=16)<br>*半年付 · 付 €37.50* | [€6.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=16)<br>*年付 · 付 €75.00* | — | — |

- Micro KVM 的 **768MB 内存**是刻意做出来的引流款：能跑 WireGuard / 静态页 / 轻量脚本，装完 Debian 剩余内存通常只有 300MB 上下。别拿它跑 Docker 或数据库。
- Advanced KVM（1C/2.5G/45G）是**唯一提供 /64 IPv6** 的 Linux 档，其余都是 /112 子网。
- DIY（Do It Yourself）支持自己拉 vCPU 1→8、内存 1→32GB、硬盘 20→500GB、流量 1→20TB，但**只有月付到年付四档，没有两年 / 三年付**，最低 €7.50/月起。

### 二、Windows RDP VPS —— 3 个档位

**Windows VPS：跑 Windows 软件的常开小机器**

三个档位分别是 Win 4G（2C/4G/60G）、Win 8G（4C/8G/120G）、Win 12G（4C/12G/160G），同样支持 11 个机房任意选。定位很明确：一台 7×24 小时开着、团队用远程桌面共享的 Windows 机器——跑没有 Linux 版的桌面软件、.NET / IIS / SQL Server，或者给工作室当常驻节点。

★ **授权要自己解决**：RareCloud 提供的是 Windows Server 模板，官方模板自带 **180 天评估期**，正式商用必须自行向微软或授权经销商购买许可证；已有 Windows Server 授权的可以自带激活。

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | IP | 月付 | 季付 | 半年付 | 年付 | 两年付 | 三年付 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| **Win 4G** | 2 vCPUs | 4GB RAM | 60GB NVMe | 4TB /month | 1x IPv4 & /112 IPv6 Subnet | [€15.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=7)<br>*月付 · 付 €15.50* | — | — | [€12.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=7)<br>*年付 · 付 €155.00* | [€12.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=7)<br>*两年付 · 付 €310.00* | [€12.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=7)<br>*三年付 · 付 €465.00* |
| **Win 8G** | 4 vCPUs | 8GB RAM | 120GB NVMe | 6TB /month | 1x IPv4 & /112 IPv6 Subnet | [€29.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=17)<br>*月付 · 付 €29.50* | — | — | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=17)<br>*年付 · 付 €295.00* | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=17)<br>*两年付 · 付 €590.00* | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=17)<br>*三年付 · 付 €885.00* |
| **Win 12G** | 4 vCPUs | 12GB RAM | 160GB NVMe | 10TB /month | 1x IPv4 & /112 IPv6 Subnet | [€34.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=18)<br>*月付 · 付 €34.50* | — | — | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=18)<br>*年付 · 付 €345.00* | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=18)<br>*两年付 · 付 €690.00* | [€28.75](https://rarecloud.io/clients/aff.php?aff=1012&pid=18)<br>*三年付 · 付 €1035.00* |

- Win 系列的计费周期也只到**三年付**，且年付 / 两年付 / 三年付同价，锁长周期没有额外折扣。
- 社区对 Windows 档位的测评样本很少，选之前建议先用 Linux 档位或 Cloud VM 试手。

### 三、n8n 自动化 VPS —— 2 个档位

**n8n VPS：预装好 n8n 与 HTTPS，开箱即用**

n8n 是自建工作流自动化的热门开源工具，官方云版按执行次数收费。RareCloud 的做法是**把 n8n、Nginx 反代、Let's Encrypt 证书、UFW 防火墙（只开 22/80/443）全部预装好**，你只需要 SSH 进去跑一句 `bash /root/setup-domain.sh yourdomain.com` 绑定域名、拿证书。

★ 这条线的**年付折扣是全站最猛的**：Starter 月付 €9.50、年付总价 €48（折合 **€4.00/月**），Pro 月付 €19.50、年付 €68.25（折合 €5.69/月）。官方也直接写「无执行次数限制」——只要 CPU 和内存扛得住就跑多少。

- Starter 用 SQLite 嵌入式数据库，适合小项目；Pro 是 Docker + PostgreSQL 16 + Redis 7 + 2 个 worker 节点的队列模式，数据库和缓存不对公网暴露。
- 注意 n8n Starter（pid 36）与 OpenClaw Server（pid 49）**价格完全一样**，Pro 与 Desktop 同理——两条线在后台共用同一套计费配置。

### 四、OpenClaw AI 助手 VPS —— 2 个档位

**OpenClaw VPS：把 AI 助手放在自己机器上**

OpenClaw 是一个开源自托管 AI 助手。RareCloud 把它和 headless Chrome 一起预装好，并按官方说法做了 **8 层安全加固**：nftables 防火墙、fail2ban、AppArmor profile、仪表盘**只监听 localhost**（要访问得走 SSH 隧道）、自动安全更新。接 Telegram / WhatsApp / Discord / Slack / Signal 都可以，模型用你自己的 Anthropic 或 OpenAI key。

Server 档从 **2C / 4GB / 65GB NVMe / 5TB** 起步，Desktop 档从 **4C / 8GB / 100GB NVMe / 7TB** 起步，后者多一套 **XFCE 图形桌面 + 非 headless 的 Chrome / Firefox**，可以从控制面板用 VNC 看 AI 实时点网页、填表单。两条线都是**可自定义配置**的。

- 对隐私敏感的用法来说这是最大卖点：**对话记录和 API key 都留在你自己的服务器上**，RareCloud 不经手。
- 「你的 AI 帮你操作浏览器」这件事本身风险不小，建议把桌面档放在带 AppArmor 的隔离环境里用。
- ⚠️ 官网自身数据打架：WHMCS 产品描述里写 Desktop 是 2C/8G/60G，而官网产品卡是 4C/8G/100GB。本文采用**官网产品卡**的数据，下单前建议以控制台实际配置为准。

### 五、Web 虚拟主机 —— 4 个档位

**Web 主机：cPanel / WordPress 一键装**

给不想碰服务器的人准备的：免费 SSL、每日备份、独立 IP，Business 及以上送域名注册。四个档位从 **Website Hosting 年付 €30（折合 €2.50/月）**起，再到 StartUp / Business / Enterprise 三档不限量站点方案。

★ 这条线有个**明显的定价 bug 值得避坑**：Enterprise 档月付 €39.50、年付 €295，但**两年付和三年付分别是 €390 / €585，和低一档的 Business 完全相同**。也就是说 Enterprise 锁长周期不但没有溢价，还比它自己月付便宜一大截——这多半是配置没同步，买之前建议先开工单问清楚。

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | IP | 月付 | 季付 | 半年付 | 年付 | 两年付 | 三年付 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| **StartUp** | 1.5 核 | 2GB RAM | 50GB NVMe | 不限流量 | 1 个网站 · 独立 IP · 送 SSL | [€9.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=21)<br>*月付 · 付 €9.50* | — | — | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=21)<br>*年付 · 付 €95.00* | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=21)<br>*两年付 · 付 €190.00* | [€7.92](https://rarecloud.io/clients/aff.php?aff=1012&pid=21)<br>*三年付 · 付 €285.00* |
| **Business** | 3 核 | 4GB RAM | 100GB NVMe | 不限流量 | 不限站点 · 独立 IP · 送 SSL + 域名 | [€19.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=22)<br>*月付 · 付 €19.50* | — | — | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=22)<br>*年付 · 付 €195.00* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=22)<br>*两年付 · 付 €390.00* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=22)<br>*三年付 · 付 €585.00* |
| **Enterprise** | 6 核 | 8GB RAM | 不限 NVMe | 不限流量 | 不限站点 · 独立 IP · 送 SSL + 域名 | [€39.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=23)<br>*月付 · 付 €39.50* | — | — | [€24.58](https://rarecloud.io/clients/aff.php?aff=1012&pid=23)<br>*年付 · 付 €295.00* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=23)<br>*两年付 · 付 €390.00* | [€16.25](https://rarecloud.io/clients/aff.php?aff=1012&pid=23)<br>*三年付 · 付 €585.00* |
| **Website Hosting** | 共享 | 共享 | 10GB NVMe | 不限流量 | 10 个邮箱 · 送 .com 域名 · 99.9% uptime | — | — | — | [€2.50](https://rarecloud.io/clients/aff.php?aff=1012&pid=51)<br>*年付 · 付 €30.00* | [€2.29](https://rarecloud.io/clients/aff.php?aff=1012&pid=51)<br>*两年付 · 付 €55.00* | [€2.22](https://rarecloud.io/clients/aff.php?aff=1012&pid=51)<br>*三年付 · 付 €80.00* |

- Website Hosting（pid 51）只有年付 / 两年付 / 三年付，没有月付，配置是 10GB NVMe、不限流量、10 个邮箱、99.9% uptime。

### 六、Cloud VM 与云附加件（布加勒斯特）

**Cloud VM：13 个规格，按小时结算**

和前面的 VPS 是两套体系：**Cloud VM 只在布加勒斯特机房**，**按小时计费、当月费用封顶在月价**，从 €3.99/月（S-1，1C/2G/25G/1TB）起，分四个家族：Cost-Optimized（S）、General Purpose（G）、CPU-Optimized（C）、Memory-Optimized（M）。官网自己给了横向对比：G-2（2C/8G/100G/6TB）€14.99/月，同规格 Hetzner CPX32 要 €35.99、DigitalOcean $42、Vultr $40。

每个 Cloud VM 都自带**公网 IPv4、NVMe 存储、云防火墙、私网**，并且支持随时改配置而不换 IP。按需付费的几项附加服务价格也公开：快照 / 云硬盘 **€0.05/GB/月**、保留 IP **€2/月**、负载均衡 **€9/月（含公网 IP）**、对象存储 **€10/月含 1TB**、K8s worker **€7.99/月起**（控制面免费）。

- Cloud 资源**先用量后付费**：月末出账，账上有余额 / 赠金会自动抵扣。欠费超过 7 天会在账单国家当地时间 09:00 关机，再过 14 天连同数据永久删除。
- 账单低于 €5 顺延到下期。**资源只要存在就计费，不管开关机**，删掉才停止计费。

#### Cloud VM 13 个规格（按小时计费，月价封顶）

| 规格 | 家族 | vCPU | 内存 | NVMe | 含流量 | 月价封顶 | 下单 |
|---|---|---|---|---|---|---|---|
| **S-1** | Cost-Optimized | 1 | 2 GB | 25 GB | 1 TB | **€3.99**<br>*€0.0055/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| **S-2** | Cost-Optimized | 2 | 4 GB | 50 GB | 2 TB | **€6.99**<br>*€0.0096/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| **S-4** | Cost-Optimized | 4 | 8 GB | 80 GB | 4 TB | **€12.99**<br>*€0.0178/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| **G-1** | General Purpose | 1 | 4 GB | 60 GB | 4 TB | **€7.99**<br>*€0.0109/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| **G-2** | General Purpose（推荐） | 2 | 8 GB | 100 GB | 6 TB | **€14.99**<br>*€0.0205/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| **G-4** | General Purpose | 4 | 16 GB | 160 GB | 8 TB | **€27.99**<br>*€0.0383/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| **G-8** | General Purpose | 8 | 32 GB | 240 GB | 12 TB | **€52.99**<br>*€0.0726/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| **C-2** | CPU-Optimized | 2 | 4 GB | 80 GB | 6 TB | **€19.99**<br>*€0.0274/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| **C-4** | CPU-Optimized | 4 | 8 GB | 120 GB | 8 TB | **€37.99**<br>*€0.0520/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| **C-8** | CPU-Optimized | 8 | 16 GB | 200 GB | 12 TB | **€72.99**<br>*€0.1000/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| **M-2** | Memory-Optimized | 2 | 16 GB | 80 GB | 6 TB | **€44.99**<br>*€0.0616/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| **M-4** | Memory-Optimized | 4 | 32 GB | 160 GB | 8 TB | **€84.99**<br>*€0.1164/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |
| **M-8** | Memory-Optimized | 8 | 64 GB | 320 GB | 12 TB | **€159.99**<br>*€0.2192/h* | [部署 →](https://rarecloud.io/clients/aff.php?aff=1012) |

#### Cloud 附加服务

| 服务 | 价格 |
|---|---|
| 快照 Snapshot | €0.05 / GB / 月，每台最多 5 个，最低 €0.25/个 |
| 块存储 Block Storage | €0.05 / GB / 月，单卷最大 2 TB，可跨机迁移 |
| 保留 IP Reserved IP | €2 / 月 |
| 负载均衡 Load Balancer | €9 / 月（含公网 IP） |
| 对象存储 Object Storage | €10 / 月含 1 TB（S3 兼容） |
| Managed Kubernetes | 控制面免费，worker 从 €7.99 / 月起 |

## 社区真实评价：NodeSeek 417 条搜索结果里都说了什么

下面是 NodeSeek 上 202 篇相关帖子的正文与评论里被反复提到的说法，每条都附原帖链接。

### 👍 被认可的地方

- **价格是真的低** — 「Rarecloud €8.3/年 德国三网直连 上海这联通电信好香。。25三年还能买」——三年付 €25 的 1C/1G/25G/3T，在当时是全网最低梯队。  
  —— NodeSeek，2025-02-02，[查看原帖](https://www.nodeseek.com/post-242618-1)
- **德国机房硬件更好** — 「综合来看，硬盘读写都差不多，德国机房硬件较好，CPU 的 GB5 分数上 1000，线路也是直连的，延迟也不错」；另一篇测评里德国机是 Ryzen 7 5800X，GB5 单核 982、SysBench 单线程 1906。  
  —— NodeSeek，2024-12-30，[查看原帖](https://www.nodeseek.com/post-213762-1)
- **移动用户有真香机** — 香港机房被反复称为「移动快乐鸡」，回程 CMI 直连、延迟低、不丢包；有用户从日本迁到香港后「用得很爽」。  
  —— NodeSeek，2025-12-20，[查看原帖](https://www.nodeseek.com/post-541236-1)
- **平时其实挺稳** — 「探针一直很稳定，基本上只有机房升级才有问题。用了两年倒没发现什么问题，工单响应挺及时」。  
  —— NodeSeek，2026-05-15，[查看原帖](https://www.nodeseek.com/post-732070-1)
- **欧盟主体、可开 VAT 发票** — 服务方是罗马尼亚公司，接受信用卡 / 借记卡、PayPal、支付宝、加密货币与银行转账，有商业用途可以走 VAT 发票。  
  —— NodeSeek，2026-10-14，[查看原帖](https://rarecloud.io/tos/)

### 👎 被吐槽的地方

- **退款极难，14 天政策形同虚设** — 「12 月 1 日买的 vps，后面申请工单退款，到现在快一个月了都没有退款成功」；工单被反复以「上报高层」为由拖延，社区共识是「一定要用 PayPal 付，支付宝没办法」。  
  —— NodeSeek，2025-12-26，[查看原帖](https://www.nodeseek.com/post-559090-1)
- **稳定性波动大** — 2026-08、2026-10 连续出现「又挂了」「失联」帖；2025-06 有人「IP 所有地方都不通」整整一天；社区结论是「欧洲节点要稳定一些，美国节点稳定性很差，经常关机或者丢包率高到没边了」。  
  —— NodeSeek，2026-10-03，[查看原帖](https://www.nodeseek.com/post-958377-1)
- **续费已经涨过一轮** — 2026-09 官方通知续费涨价：25 欧三年付涨到 37.5 欧三年付；有用户反馈「我的从大概 25o 一年变成 100o 一年」。另据邮件，Pro VPS (VM9) 自 **2028-01-24** 起为 $113.25/年（当前标价 $226.49，保留 50% 折扣）。  
  —— NodeSeek，2026-09-07，[查看原帖](https://www.nodeseek.com/post-916089-1)
- **充值赠金是陷阱** — 「25 欧元以下，充多少，送多少……续费时，最多且只能续一个周期，如果之前就续费过，现在连第一个周期都没结束，那根本没法用赠金去续费」，而且赠金**只有 60 天有效期**。社区把「50o 翻 3 倍」直接当作高风险信号。  
  —— NodeSeek，2026-09-05，[查看原帖](https://www.nodeseek.com/post-888388-1)
- **强制迁移会换 IP** — 2025-12 荷兰节点整体迁到海牙新机房，退役 45.129.13.0/24、45.148.11.0/24、45.142.192.0/24，迁移后**全部换新 IP**；硅谷节点同样退役多个 /24。条款也写明 IP 不可迁移、不可转让，商家可改号。  
  —— NodeSeek，2025-12-14，[查看原帖](https://www.nodeseek.com/post-530431-1)
- **老款可能被降配** — 有用户翻出一台三年前的老机重测：「单核 5800x 被干成了 9254」「内存也降了，只有 1.5G 了」——商家在基础设施迁移后把老机器换到了新硬件上。  
  —— NodeSeek，2026-06-14，[查看原帖](https://www.nodeseek.com/post-763050-1)
- **IP 质量与流媒体** — 「不要指望解锁，广播 IP，Gemini 给你飞罗马尼亚，或者送美送中，chatgpt 直接显示你是 VPN」。  
  —— NodeSeek，2026-05-15，[查看原帖](https://www.nodeseek.com/post-732070-1)
- **商家自己不做备份** — 条款写明：除非服务协议另有说明，RareCloud **不做任何客户数据备份**，数据丢失概不负责。系统盘损坏需要用户自己扛。  
  —— NodeSeek，2026-10-14，[查看原帖](https://rarecloud.io/tos/)

## ⚠️ 购买前必读：6 条风险提示

RareCloud 的价格优势是真的，社区对它稳定性和续费政策的质疑也是真的。下面 6 条全部来自官方条款原文或 NodeSeek 原帖。

1. **先充值还是先开机？——先开机，别囤赠金**  
   充值赠金 60 天过期，且续费一次只能消耗一个周期。你手上的 VPS 越早开、周期排得越靠前，赠金越用得上；反过来先充值再慢慢开机，赠金大概率白瞎。
2. **锁多久合适？——最稳的是 1 年，最多 2 年**  
   年付比月付便宜 15%–17%，三年付再便宜一档；但 2026-09 已经涨过一轮、条款也没有长期锁价承诺。Plus / Pro / Win 系列**两年付和三年付同价**，锁三年纯属多担风险。
3. **迁移风险要自己消化**  
   历史已发生三次大规模迁移（荷兰→海牙、硅谷换 IP 段、老机换硬件）。TOS 明确「IP 是服务的一部分，不可携带、不可转让，商家改号会尽力避免中断」。所以 DNS 记录别写死，有条件就用 Cloudflare 之类的托管解析。
4. **付款方式决定了你的退路**  
   官方支持 PayPal、信用卡 / 借记卡、支付宝、加密货币、银行转账。**社区的一致建议是优先用 PayPal**——支付宝订单几乎没有成功退款的先例。
5. **价格不含 VAT**  
   官网价格全部是**不含税**价。欧盟客户若无有效 VAT ID，会被加收 **19% 罗马尼亚增值税**；中国大陆用户在结账前务必确认最终应付金额。
6. **别把它当生产主力**  
   99.9% uptime 的 SLA 是写在条款里的（低于阈值可按 downtime 的 10%/1% 申请退月费，需开工单），但 SLA 赔付和退款一样要看客服脸色。生产业务建议：**年付一台 + 自己做快照 + 有兜底方案**。

## 常见问题

**RareCloud 是什么来头？靠谱吗？**  
运营方是罗马尼亚的 RARE MOOD AGENCY SRL（Tax ID 45192771，VAT RO45192771），背后是罗马尼亚持牌电信运营商 M247（AS9009），12 个机房里有 7 个直接挂在 M247 的 AS9009 下。它不是空壳新号，但确实是**近两年在社区里争议很大的低价商家**——「价格真香」和「随时可能跑路」两种评价同时存在。建议按年付玩具 / 副业机器的定位买。

**最便宜多少钱？**  
€1.56/月——Micro KVM（1 vCPU / 768MB / 15GB NVMe / 1TB 流量），**一次付三年 €56**。注意 Micro 和 Starter **没有月付**，最低一次性付 1.5 年。

**可以按月付吗？**  
Linux KVM 里 Advanced / Core / DIY / Plus / Pro / Elite 和全部 Windows、n8n、OpenClaw 档位都可以月付；**只有 Micro KVM、Starter KVM、Website Hosting 三档没有月付**。Cloud VM 全部按小时计费、封顶月价。

**中国大陆用户选哪个机房？**  
**移动选香港**（回程 CMI 直连，社区称「移动快乐鸡」）；**电信 / 联通选德国**（三网回程 4837 直连，延迟约 180–260ms）；**电信不要选香港和东京**，回程绕路、丢包明显。

**怎么验证线路好不好？**  
每个机房官网页面都直接给了 test IP，例如法兰克福 `85.121.52.2`、伦敦 `85.121.48.2`、东京 `85.121.50.2`、香港 `85.121.244.250`。下单前先 `ping` 和 `mtr` 测一下再付钱。

**支持支付宝吗？**  
支持。官方条款列出的支付方式是信用卡 / 借记卡、PayPal、**支付宝**、加密货币和银行转账。但社区一致提醒：**想退款就用 PayPal 付**，支付宝单几乎没成功退款的。

**有备份吗？**  
没有。条款明确写了除非另有说明，RareCloud 不为客户数据做备份，硬件故障、误操作导致的数据丢失概不负责。Cloud VM 有快照服务（€0.05/GB/月，每台最多 5 个），KVM VPS 档位得自己解决备份。

**退款政策是怎样的？**  
条款写的是 **14 天退款**（需满足「使用量极少」等条件），超出后按 as-is 处理，除非 30 天内换机或转余额。但社区反馈是：工单经常只回复「已上报高层」，有人退款拖了两个月，最后靠 **PayPal 争议**秒退。

**IP 会被换掉吗？**  
会。历史上荷兰节点从原机房迁到海牙时**整段 IP 全换**（退役 45.129.13.0/24、45.148.11.0/24、45.142.192.0/24），硅谷节点也退役过多个 /24。条款明确 IP 不可迁移、不可转让。建议用第三方托管 DNS，别把解析挂在会变动的 IP 上。

**能解锁流媒体吗？**  
基本别指望。有用户直接反馈「Gemini 定位飞到罗马尼亚，ChatGPT 直接判定为 VPN」，属于广播 IP。需要解锁请另找专门的 IP 商家。

## 数据来源与免责声明

- RareCloud 官网 Linux VPS 页：<https://rarecloud.io/kvm-vps/>
- RareCloud 官网 Cloud VM 页（13 档规格与横向对比）：<https://rarecloud.io/cloud-vm/>
- RareCloud 官网数据中心页（12 机房 / ASN / transit / IX / test IP）：<https://rarecloud.io/datacenters/>
- RareCloud 服务条款（SLA、退款、备份、IP、VAT）：<https://rarecloud.io/tos/>
- RareCloud 联盟计划（15% 持续佣金）：<https://rarecloud.io/affiliates/>
- 定价数据源（WHMCS 导出，2026-10-14 04:00 快照）：<https://rarecloud.io/data/whmcs-pricing.json>
- NodeSeek 搜索「rarecloud」9 页共 417 条结果：<https://www.nodeseek.com/search?q=rarecloud>
- NodeSeek 202 篇相关帖子正文与 1761 条评论：<https://www.nodeseek.com/>

本文引用的 28 条来源帖、202 篇抓取正文与 1761 条评论，可在 `data/rarecloud-来源帖映射.json` 与 `data/nodeseek-帖子正文与评论-rarecloud.json` 中复核。

**免责声明：**价格与库存均为 2026-10-14 抓取时点快照，随时可能变动；本文含 `aff=1012` 推广链接，商家按每次续费向我支付 15% 佣金，不额外向你收费。本文不构成购买建议，请结合自身风险承受能力判断。
