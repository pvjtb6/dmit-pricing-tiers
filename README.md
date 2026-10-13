# DMIT 性价比：洛杉矶/香港/东京全套餐价格拆解，哪一档值得买、哪一档可以跳过

搜「DMIT 性价比」的人，多半已经翻过一轮价格表，然后被两个数字同时卡住：洛杉矶 Tier 1 年付 $36.9，便宜得不像这家靠 CN2 GIA 出名的商家；香港 Premium 起步 $39.9/月，又贵得让人怀疑自己是不是看错了小数点。两个数字都是真的，差在线路。

DMIT 把产品按网络质量切成三段——Premium（CN2 GIA）、Eyeball（CMIN2 + 9929）、Tier 1（纯国际 BGP）。同一台机器、同一个机房，换一条线路，价格能差三倍。所以「DMIT 划不划算」这道题没有统一答案，只有「这一档对你划不划算」。

下面把三条线路、三个机房的价格摆在一起，顺便说清楚哪些档位是真便宜，哪些档位多花的钱买的是你大概率用不上的东西。

## 先分清三条线路，再决定看哪张表

线路选错，套餐再便宜也是浪费。三档的区别很具体：

- **Premium（Pro）**：电信去程 CN2 GIA，联通去程 AS4837，移动去程经香港移动，三网回程统一走 CN2 GIA（AS4809）。对电信用户最友好，也是定价最高的一档。
- **Eyeball（EB）**：电信在 AS9929 与 AS58807 之间负载分配，联通主要走 AS9929，移动主要走 CMIN2。移动和联通体验接近 Pro，电信不如 Pro 稳，但同价位给到的流量通常更多。
- **Tier 1（T1）**：国际 BGP 路由，完全没有中国大陆方向的优化。香港 T1 接入 RETN 一类的国际骨干，但电信用户用它访问内地，延迟有可能比美西还难看。

一句话判断：**你的用户在国内、主要是电信宽带，看 Pro；用户在国内、以移动为主，看 EB；用户根本不在国内，看 T1。**

## 洛杉矶（LAX）全套餐价格表：AS3 平台

DMIT 洛杉矶目前有 AS3（AMD EPYC 7003）、AN4（EPYC 9004）、AN5（EPYC 9005）三个硬件平台并存，同一档套餐换平台价格会往上跳，下面先把价格最低、最常被当作「性价比入口」的 AS3 全部列出来。

### Premium 系列（三网回程 CN2 GIA）

| 套餐 | CPU / 内存 / 硬盘 | 流量与端口 | 超量后 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- |
| LAX.AS3.Pro.TINY | 1 核 / 2GB / 20GB SSD | 1TB @ 1Gbps | 4Mbps 不限流 | $10.90/月 | [ 直达该套餐下单页](https://www.dmit.io/cart.php?aff=12046&region=los-angeles&generation=as3&network=premium&product=lax.as3.pro.tiny) |
| LAX.AS3.Pro.Pocket | 2 核 / 2GB / 40GB SSD | 1.5TB @ 4Gbps | 4Mbps 不限流 | $16.90/月 | [ 查看 Premium 线路套餐](https://www.dmit.io/cart.php?aff=12046&region=los-angeles&generation=as3&network=premium) |
| LAX.AS3.Pro.STARTER | 2 核 / 2GB / 80GB SSD | 3TB @ 10Gbps | 4Mbps 不限流 | $34.90/月 | [ 查看 Premium 线路套餐](https://www.dmit.io/cart.php?aff=12046&region=los-angeles&generation=as3&network=premium) |
| LAX.AS3.Pro.MINI | 4 核 / 4GB / 80GB SSD | 5TB @ 10Gbps | 8Mbps 不限流 | $62.90/月 | [ 查看 Premium 线路套餐](https://www.dmit.io/cart.php?aff=12046&region=los-angeles&generation=as3&network=premium) |
| LAX.AS3.Pro.MICRO | 4 核 / 4GB / 160GB SSD | 7TB @ 10Gbps | 8Mbps 不限流 | $87.90/月 | [ 查看 Premium 线路套餐](https://www.dmit.io/cart.php?aff=12046&region=los-angeles&generation=as3&network=premium) |
| LAX.AS3.Pro.MEDIUM | 6 核 / 8GB / 160GB SSD（2 个 IPv4） | 14TB @ 10Gbps | 10Mbps 不限流 | $199.90/月 | [ 查看 Premium 线路套餐](https://www.dmit.io/cart.php?aff=12046&region=los-angeles&generation=as3&network=premium) |

### Eyeball 系列（CMIN2 / 9929 优化）

| 套餐 | CPU / 内存 / 硬盘 | 流量与端口 | 超量后 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- |
| LAX.AS3.EB.TINY | 1 核 / 2GB / 20GB SSD | 1.5TB @ 2Gbps | 4Mbps 不限流 | $10.90/月 | [ 查看 Eyeball 线路套餐](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.EB.Pocket | 2 核 / 2GB / 40GB SSD | 3TB @ 4Gbps | 4Mbps 不限流 | $16.90/月 | [ 查看 Eyeball 线路套餐](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.EB.STARTER | 2 核 / 2GB / 80GB SSD | 5TB @ 10Gbps | 4Mbps 不限流 | $34.90/月 | [ 查看 Eyeball 线路套餐](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.EB.MINI | 4 核 / 4GB / 80GB SSD | 10TB @ 10Gbps | 8Mbps 不限流 | $62.90/月 | [ 查看 Eyeball 线路套餐](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.EB.MICRO | 4 核 / 4GB / 160GB SSD | 14TB @ 10Gbps | 8Mbps 不限流 | $87.90/月 | [ 查看 Eyeball 线路套餐](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.EB.MEDIUM | 6 核 / 8GB / 160GB SSD | 30TB @ 10Gbps | 10Mbps 不限流 | $199.90/月 | [ 查看 Eyeball 线路套餐](https://www.dmit.io/aff.php?aff=12046) |

### Tier 1 系列（国际 BGP，无中国大陆优化）

| 套餐 | CPU / 内存 / 硬盘 | 流量与端口 | 超量后 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- |
| LAX.AS3.T1.WEE | 1 核 / 1GB / 20GB SSD | 1TB @ 4Gbps | 100Mbps 不限流 | $36.90/年 | [ 查看 Tier 1 线路套餐](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.T1.TINY | 1 核 / 1GB / 20GB SSD | 2TB @ 4Gbps | 200Mbps 不限流 | $6.90/月 | [ 查看 Tier 1 线路套餐](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.T1.STARTER | 1 核 / 2GB / 40GB SSD | 4TB @ 10Gbps | 200Mbps 不限流 | $12.90/月 | [ 查看 Tier 1 线路套餐](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.T1.MINI | 2 核 / 2GB / 60GB SSD | 8TB @ 10Gbps | 200Mbps 不限流 | $21.90/月 | [ 查看 Tier 1 线路套餐](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.T1.MICRO | 4 核 / 4GB / 80GB SSD | 16TB @ 10Gbps | 500Mbps 不限流 | $32.90/月 | [ 查看 Tier 1 线路套餐](https://www.dmit.io/aff.php?aff=12046) |

Eyeball 和 Tier 1 的推广链接没有可以直接定位到单一档位的页面，点进去会落到 DMIT 的套餐入口，在 **Routing Profile** 里切到对应线路，就能看到该线路下的全部机型。Premium 的 TINY 档可以直接落到具体商品页。

## 换到 AN5 平台，同样的配置要多花多少

AN5 用的是 AMD EPYC 9005，CPU 更新一代，价格也跟着往上走。以洛杉矶 Premium 为例：

| 档位 | AS3 平台 | AN5 平台 | 差价 |
| --- | --- | --- | --- |
| TINY | $10.90/月 | $14.90/月 | +$4 |
| Pocket | $16.90/月 | $21.90/月 | +$5 |
| STARTER | $34.90/月 | $43.90/月 | +$9 |
| MINI | $62.90/月 | $79.90/月 | +$17 |
| MICRO | $87.90/月 | $110.90/月 | +$23 |
| MEDIUM | $199.90/月 | $289.90/月 | +$90 |
| LARGE（8 核 / 16GB / 320GB / 25TB） | — | $499.90/月 | — |
| GIANT（12 核 / 24GB / 640GB / 50TB） | — | $1009.90/月 | — |

看这组数字就明白一件事：MINI 以上换平台，多付的是纯 CPU 代际溢价。除非你跑的是能吃满单核性能、且性能直接换成钱的任务（比如高并发的编译、转码、实时计算），否则 $17 到 $90 的差价很难在日常建站场景里找回来。[👉 对比 AS3 与 AN5 的实时报价](https://www.dmit.io/cart.php?aff=12046&region=los-angeles&generation=an5&network=premium)

## 香港和东京：贵在哪，什么时候才值得买

香港机房的物理位置决定了它对内地的天然优势，也决定了它的价格不会友好。同样一条 Premium 线路，香港起步就是 $39.9/月，是洛杉矶 TINY 的将近四倍。

| 机房 / 线路 | 套餐 | 配置摘要 | 价格 | 购买 |
| --- | --- | --- | --- | --- |
| 香港 Tier 1 | HKG.T1.WEE | 1 核 / 1GB / 20GB，1TB @ 4Gbps，超量 50Mbps | $36.90/年 | [ 查看香港套餐](https://www.dmit.io/aff.php?aff=12046) |
| 香港 Tier 1 | HKG.T1.TINY | 1 核 / 1GB / 20GB，2TB | $6.90/月 | [ 查看香港套餐](https://www.dmit.io/aff.php?aff=12046) |
| 香港 Tier 1 | HKG.T1.STARTER | 1 核 / 2GB / 40GB，4TB | $12.90/月 | [ 查看香港套餐](https://www.dmit.io/aff.php?aff=12046) |
| 香港 Premium | HKG.Pro.TINY | 1 核 / 1GB / 20GB，约 500GB @ 1Gbps | $39.90/月 | [ 查看香港套餐](https://www.dmit.io/aff.php?aff=12046) |
| 东京 Tier 1 | TYO.T1.WEE | 1 核 / 1GB / 20GB，约 600GB @ 1Gbps | $36.90/年 | [ 查看东京套餐](https://www.dmit.io/aff.php?aff=12046) |
| 东京 Premium | TYO.Pro.TINY | 1 核 / 1GB / 20GB，约 300GB @ 100Mbps | $21.90/月 | [ 查看东京套餐](https://www.dmit.io/aff.php?aff=12046) |

香港 Premium 中高配已经陆续切到 AN5 平台，价格波动比洛杉矶更大；东京 Eyeball 系列据第三方反馈长期处于下架或缺货状态，东京 Premium 也需要盯着补货。这两个机房值得买的逻辑其实很简单：**你的业务必须落在香港或东京，而且用户对延迟敏感**。如果只是想要一个亚洲 IP 但不在意国内访问质量，两地的 Tier 1 年付款会便宜得多。

## 性价比排序：真正值得下手的档位就几个

把三条线路放在一起比，结论比想象中集中。

**第一梯队：LAX 的 T1.WEE（$36.90/年）。** 折算下来每月 $3 出头，1 核 1GB、1TB 流量、4Gbps 端口，流量跑完还能在 100Mbps 上继续不限流跑。同价位别家基本只能买到小厂的普通线路。前提是它的用户不在国内——拿它跑面向海外的站点、中转、监控、机器人这类轻负载，是 DMIT 全站单价最低的组合。要注意这一档基本不参与优惠码。

**第二梯队：Pro.TINY 和 EB.TINY（同为 $10.90/月）。** 这是「花得不多、但真的用上了 CN2 GIA / CMIN2」的入门点。两者同价，EB 给的流量是 1.5TB、端口 2Gbps，Pro 是 1TB、端口 1Gbps。所以：**移动用户直接选 EB.TINY，性价比更直观；电信用户多花的钱买的是回程线路质量，值不值取决于你对跨境延迟有多敏感。**

**第三梯队：EB.Pocket（$16.90/月）。** 多加 $6，从 1 核 2GB 升到 2 核 2GB，流量从 1.5TB 涨到 3TB，端口从 2Gbps 到 4Gbps。这是全表里配置涨幅最明显的一跳，拿它跑正经的个人站点或小型应用，比在 TINY 上硬撑要合理。

再往上就要想清楚了。Pro 和 EB 的 STARTER 都是 $34.90/月，CPU 和内存和 Pocket 完全一致，多出来的钱买的是 10Gbps 端口和更多流量；MINI 到 $62.90/月 才真正加核心和内存。**如果你的站点每月流量还在几百 GB 量级，STARTER 及以上付出的带宽溢价基本是闲置的。**

## 优惠码：能省多少，怎么用

DMIT 的促销风格和它的定价风格一致——不搞大促，优惠码数量少、绑定条件严，而且多数只对特定线路和特定付款周期生效。下面这些来自第三方整理和官方历史促销记录，**能否使用必须在结算页点 Validate Code 验证**：

| 优惠码 | 适用范围 | 力度 |
| --- | --- | --- |
| `LAX-EB-LAUNCH-NON-MONTHLY-RECURRING-20OFF` | 洛杉矶 Eyeball，非月付 | 8 折，循环 |
| `202510_HKG_TYO_PRO_20OFF_RECURRING` | 香港 / 东京 Premium，季付及以上 | 8 折，循环 |
| `202510_HKG_TYO_T1_30OFF_RECURRING` | 香港 / 东京 Tier 1，季付及以上（不含 WEE） | 7 折，循环 |
| `2025-TYO-T1-HI-GSL-NON-MONTHLY-30OFF` | 东京 Tier 1，季付及以上 | 7 折 |
| `Lite-Annually-Recur-30OFF` | Standard / Lite 系列年付 | 7 折 |
| `Lite-Semi-Annually-Recur-20OFF` | Standard / Lite 系列半年付 | 8 折 |
| `HKG-Lite-LAUNCH-NON-MONTHLY-RECURRING-20OFF` | 香港 Lite 系列，非月付 | 8 折，循环 |
| `2025-XMAS-LAX-PRO-EB-ANNUALLY-STARTER-AND-HIGHER-15OFF-RECURRING` | 洛杉矶 Pro / EB，年付 STARTER 及以上 | 85 折 + 返现 |
| `2025-XMAS-LAX-PRO-EB-10-OFF-RECURRING` | 洛杉矶 Pro / EB 常规套餐 | 9 折 + 返现 |
| `2025-XMAS-LAX-T1-10-OFF-RECURRING` | 洛杉矶 Tier 1（不含 WEE） | 9 折 + 返现 |

用法很直接：选好套餐和付款周期，在结算页填码后点 Validate Code，通过才会显示折后价。几个码之间通常不能叠加，而 WEE 档和月付订单在多个码里被明确排除。如果手里的码提示无效，说明活动已结束，别硬试。[👉 到结算页试一下当前可用的优惠码](https://www.dmit.io/aff.php?aff=12046)

## 下单前值得多花两分钟确认的几件事

**库存比价格更需要盯。** DMIT 的套餐经常整批售罄，尤其是洛杉矶 AS3 的低价档、东京 Premium 和香港 Eyeball。看着有货的页面，刷新一下可能就没了。洛杉矶 AS3 平台官方还提示过仍处于持续优化阶段，磁盘性能和 SLA 可能不如成熟平台，跑重要业务前建议先小额测试。

**流量超了不会停机。** 这一点对性价比的影响被很多人忽略：所有档位超量后都是限速继续跑，Pro/EB 大概 4–10Mbps，Tier 1 能到 100–500Mbps。也就是说 T1 的低价套餐实际上给的是「不限量 + 限速」的组合。

**支付方式对国内用户友好。** 支付宝、PayPal、信用卡都能用，不必为了买一台 VPS 专门折腾外币卡。

## 几个被问得最多的问题

**月付还是年付？** 年付单价更低，而且年付专属的优惠码更多；但 DMIT 库存变化快、平台批次也在切换，第一次买建议先用月付把线路试明白，确认延迟和路由符合预期再续年付。

**Pro 和 Eyeball 到底差多少？** 账面上只差一条线路，实际是「电信全程 CN2 GIA」和「电信走 9929 / 移动走 CMIN2」的区别。电信宽带用户对跨境抖动敏感的话，Pro 的溢价是有意义的；移动用户选 EB，同样的钱能拿到更多流量。

**Tier 1 能不能用来做国内访问？** 不建议。它没有中国大陆方向的优化，拿来跑面向海外用户的站点、开发测试环境、中转或者只要一个美国原生 IP 的用途才是它的定位。

**换硬件平台值不值？** 参考前面 AN5 与 AS3 的差价表。除非 CPU 性能直接决定你的收入，否则同样的钱升级到 EB 的更高档位、或者拉长付款周期拿折扣，回报都比换平台明显。

**IP 被墙了怎么办？** 第三方整理里流传的说法是 15 天内可免费更换一次，其他情况 $5 一次。这属于社区信息，官方页面并没有给出同等明确的说明，买之前直接问客服确认一遍更稳妥。
