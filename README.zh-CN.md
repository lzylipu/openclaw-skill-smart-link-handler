# 智能链接处理

**[English](./README.md) | [中文](./README.zh-CN.md)**

自动识别夸克/YouTube/B站链接并触发下载。

## 功能

- 夸克分享链接自动转存（通过 QAS）
- YouTube/B站视频下载（通过 MeTube）
- 剧集匹配（E01、E02…）
- aria2 批量下载集成

## 前置条件

| 变量 | 说明 |
|------|------|
| QAS_ENDPOINT | QAS 服务地址 |
| QAS_TOKEN | QAS API 令牌 |
| ALIST_ENDPOINT | Alist 服务地址 |
| ALIST_TOKEN | Alist 认证令牌 |
| ARIA2_ENDPOINT | aria2 RPC 地址 |
| ARIA2_TOKEN | aria2 RPC 令牌 |

## 用法

```bash
# 下载指定集数
python3 scripts/quark-download.py "share_link" E01 E05 E10

# 下载全部
python3 scripts/quark-download.py "share_link"

# 任务管理
python3 scripts/quark-download.py --list
python3 scripts/quark-download.py --clear
```

## License

MIT
