# idrive-apps-update

iDrive Apps 的**自更新清单**仓库。App 里「设置软件更新地址」填下面这条，就能自动检查新版本：

```
https://raw.githubusercontent.com/zhen623/idrive-apps-update/main/update.json
```

`update.json` 的字段：

| 字段 | 含义 |
| --- | --- |
| `version` | 新版本号，比手机上的高才会提示更新 |
| `url` | 新版 APK 的直链（目前放在 `aka.doubaocdn.com`） |
| `sha256` | APK 的 sha256，可核对下载是否完整 |
| `notes` | 更新说明 |

注意：GitHub 的 `main` 分支地址有 CDN 缓存（raw 约 5 分钟、jsDelivr `@main` 约 12 小时）。App 1.9.2 起改为先直连原地址，拿到的是最新内容。
