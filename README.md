# xingtu-bot · Bot 形态案例集

> 本地构建中 · 尚未推送公开。本仓只收录公开可核对的 Bot 项目与形态拆解，不是某个 Bot 产品的官方仓库。

[![License: MIT](https://img.shields.io/badge/License-MIT-orange.svg)](./LICENSE) ![状态](https://img.shields.io/badge/状态-本地构建-lightgrey)

## 一句话定位

拆解「有长期记忆、多 Bot 分工、群聊接力、外接聊天渠道」这一类 Bot 形态是怎么搭起来的——记录设计取舍与成本结构，不做产品测评排行。

## 灵感来源与边界

Grok Bot 把「一队带名字、带电脑、定时干活的 Bot」做成了付费产品。开源社区随后出现多条平替路线。本仓关注的是**这些形态背后的工程取舍**，不是替谁站台：

- 多 Bot 的记忆如何持久化、上限在哪；
- 群聊里谁先说话、谁保持沉默，如何省 token；
- Bot 如何调用本机已有的编程 Agent，而不是重新造模型；
- 数据留在谁的机器上、成本由谁承担。

## 与相邻仓的边界

| 仓 | 管什么 | 不管什么 |
|---|---|---|
| `xingtu-super-agent` | 跨 Agent 协作的控制平面与协议设计 | 不逐个拆解具体 Bot 产品 |
| **xingtu-bot**（本仓） | Bot 形态的公开案例拆解与机制记录 | 不做方法论旗舰、不做技能库 |
| `teamai-harness` | 团队 AI 配置 SSoT（skills/rules/agents 装配） | 不记录外部开源 Bot 案例 |

## 核心内容

- **形态对照**：长期记忆、主 Bot 统筹、[PASS] 沉默、外部渠道接入等机制的横向对照。
- **案例卡**：每个公开项目一张卡，写清作者、协议、安装形态、成本结构、核对日期。
- **取舍笔记**：一个设计为什么这样选、代价是什么、什么场景下不成立。


## 归属与导航

本仓属于[行途 XingTu 开源矩阵](https://github.com/xingtu1996)的案例集分区，主题独立维护；[名片仓](https://github.com/xingtu1996)只做索引，不复制本仓内容。

案例集分四仓，按边界分工、互相引用：

- [xingtu-testting](https://github.com/xingtu1996/xingtu-testting) · AI 测试
- [xingtu-bot](https://github.com/xingtu1996/xingtu-bot) · Bot 形态
- [xingtu-agent](https://github.com/xingtu1996/xingtu-agent) · Agent 落地
- [xingtu-bci](https://github.com/xingtu1996/xingtu-bci) · 协作坏例

## 快速开始

```bash
git clone <仓库地址> xingtu-bot
cd xingtu-bot
# 案例模板 cases/_TEMPLATE.md；已收录的公开案例在 cases/public/
```

新增案例先读 [`cases/_TEMPLATE.md`](cases/_TEMPLATE.md)。公开案例一律标 `public-source` 并带原文链接与核对日期；已在本机装过并实测的才可标 `verified`。

## 案例状态标注（全仓统一）

| 状态 | 含义 |
|---|---|
| `design` | 仅设计/设想，未验证 |
| `public-source` | 公开资料整理，非本仓实测，带链接与核对日期 |
| `verified` | 本机实测，有可核对证据 |
| `production` | 生产环境在用 |

## 入库规范

- 只写公开可核对的项目；不把公开演示当作本机实测，不编造提效数字。
- 名称相近但不同的项目（如两个 DeepSeek Bot）必须分开，写清安装包名与协议，避免误导。
- 价格、星标数会过时，只写「核对日期 + 以官方页面为准」，不作为长期判据。
- 实体脱敏：客户名、人名、内网域名、内部平台链路不入库。

## 许可证

[MIT](./LICENSE) · 行途 XingTu

## 作者与联系

行途 XingTu（工程署名）· 微信搜索关注：**行途技术手记**
