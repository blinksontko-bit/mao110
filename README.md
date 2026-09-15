# 骗子记录库（scam_reports）

本仓库由 Telegram 反诈机器人（mao110 / Lantern）**自动导出**，是骗子/诈骗记录的数据库快照。

> ⚠️ 数据含个人身份信息（TG ID、钱包、描述等），仅用于反诈与追溯，请勿滥用或公开传播。

## 目录结构

| 文件 | 说明 |
| --- | --- |
| `manifest.json` | **索引**（总条数、块数、导出时间、各块 raw 地址）——外部调用方从这里入手 |
| `block_NNN.json` | 分块数据（每块 base64 ≤ 95KB，条数按大小自适应） |

## 分块列表（共 3 块 / 11214 条）

| 块 | raw 地址 |
| --- | --- |
| 1 | [block_001.json](https://raw.githubusercontent.com/blinksontko-bit/mao110/main/block_001.json) |
| 2 | [block_002.json](https://raw.githubusercontent.com/blinksontko-bit/mao110/main/block_002.json) |
| 3 | [block_003.json](https://raw.githubusercontent.com/blinksontko-bit/mao110/main/block_003.json) |

## 记录字段

`id` `sourceMsgId` `channelMsgId` `channelMsgIds[]` `channelLink` `nickname` `username` `tgid` `permLink` `wallet` `amount` `description` `reporterId` `reporterUsername` `reporterNickname` `createdAt`

---
_导出时间：2026-09-15T07:30:32.224Z · 由 mao110 机器人自动生成_