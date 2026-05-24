# hitokoto-sign-plugin

云崽/LLOneBot 自动签名插件，自用。

> [!TIP]
> 一言 API：[https://v1.hitokoto.cn](https://v1.hitokoto.cn)

> [!WARNING]
> 仅支持 LLOneBot / NapCatQQ 等 OneBot11 协议端

## 目录结构

```
hitokoto-sign-plugin/
├── app/
│   └── autosign.js          # LLOneBot 版本（主入口）
├── example/
│   └── napcat自动说说2.0.js  # Napcat 版本（参考示例）
└── README.md
```

| 文件 | 协议端 | 指令前缀 | 说明 |
|---|---|---|---|
| `app/autosign.js` | LLOneBot | `#一言` | 签名更新 + 私聊推送 |
| `example/napcat自动说说2.0.js` | Napcat | `#nap` | 签名 + 说说发送 |

## 安装与更新 🔧

### TRSS-Yunzai / Yunzai-Bot 🚀

```bash
git clone --depth=1 https://github.com/GithubMrDior/hitokoto-sign-plugin ./plugins/hitokoto-sign-plugin/
```

### 安装依赖 📦

```bash
pnpm install --filter=hitokoto-sign-plugin
```

## 功能说明

- **自动更新签名**：定时获取一言，自动更新 QQ 个性签名
- **自动推送说说**：定时私聊推送一言内容（LLOneBot 暂不支持 Qzone）
- **指令控制**：支持开启/关闭、立即更新、修改定时等

## 常用指令

| 指令 | 说明 |
|---|---|
| `#一言帮助` | 查看帮助 |
| `#一言签名开启/关闭` | 开关签名更新 |
| `#一言说说开启/关闭` | 开关说说推送 |
| `#一言立即更新签名` | 立即更新签名 |
| `#一言立即更新说说` | 立即推送说说 |
| `#设置签名时间 cron表达式` | 修改签名频率 |
| `#设置说说时间 cron表达式` | 修改推送频率 |
| `#一言插件状态` | 查看当前状态 |

## Cron 表达式说明

| 效果 | 表达式 |
|---|---|
| 每小时 | `0 0 * * * *` |
| 每2小时 | `0 0 */2 * * *` |
| 每6小时 | `0 0 */6 * * *` |
| 每天12点 | `0 0 12 * * *` |
| 每30分钟 | `0 */30 * * * *` |

## 加速地址

1. https://gh-proxy.com/
2. https://ghfast.top/

## 贡献者 👨‍💻

[GithubMrDior](https://github.com/GithubMrDior)
