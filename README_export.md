# 骗子记录库（scam_reports）导出说明

本仓库由 Telegram 反诈机器人（mao110 / Lantern）**自动导出**，是骗子/诈骗记录的数据库快照。

> ⚠️ 数据含个人身份信息（TG ID、钱包、描述等），仅用于反诈与追溯，请勿滥用或公开传播。

> 📦 全量数据按大小分块（每块 base64 ≤ 95KB）。外部调用方读 `manifest.json` 拿块列表，拼合各块 `reports[]` 即全量。

## 文件位置

| 文件 | 位置 | 说明 |
| --- | --- | --- |
| `manifest.json` | **仓库根** | 索引（总条数、块范围、各块 raw 地址） |
| `README_export.md` | **仓库根** | 本说明 |
| `block_NNN.json` | `data/` | 分块数据 |

## 分块列表（共 5 块 / 11214 条）

| 块 | raw 地址 |
| --- | --- |
| 80 | [block_080.json](https://raw.githubusercontent.com/blinksontko-bit/mao110/main/data/block_080.json) |
| 81 | [block_081.json](https://raw.githubusercontent.com/blinksontko-bit/mao110/main/data/block_081.json) |
| 82 | [block_082.json](https://raw.githubusercontent.com/blinksontko-bit/mao110/main/data/block_082.json) |
| 83 | [block_083.json](https://raw.githubusercontent.com/blinksontko-bit/mao110/main/data/block_083.json) |
| 84 | [block_084.json](https://raw.githubusercontent.com/blinksontko-bit/mao110/main/data/block_084.json) |

## 记录字段

`id` `sourceMsgId` `channelMsgId` `channelMsgIds[]` `channelLink` `nickname` `username` `tgid` `permLink` `wallet` `amount` `description` `reporterId` `reporterUsername` `reporterNickname` `createdAt`

---
_导出时间：2026-09-15T09:40:10.939Z · 由 mao110 机器人自动生成_