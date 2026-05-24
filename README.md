# hitokoto-sign-plugin

云崽/LLOneBot 自动签名插件，自用。

> [!TIP]
> 一言 API：[https://v1.hitokoto.cn](https://v1.hitokoto.cn)

> [!WARNING]
> 仅支持 LLOneBot / NapCatQQ 等 OneBot11 协议端

## 安装与更新 🔧

### TRSS-Yunzai / Yunzai-Bot 🚀

```bash
git clone --depth=1 https://github.com/GithubMrDior/hitokoto-sign-plugin ./plugins/hitokoto-sign-plugin/
```

> 使用 Release 🔧

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

## 加速地址

1. https://gh-proxy.com/
2. https://ghfast.top/

## 贡献者 👨‍💻

[GithubMrDior](https://github.com/GithubMrDior)
