# legado-shuyuan

Legado（阅读 App）书源。

## 搬山人小说网

- 站点：https://www.banshanren.com
- 功能：搜索、详情、目录、正文、发现页（8 个分类，支持翻页）
- 规则已按现站结构实测（搜索/详情/目录 9 章/正文 172 段/发现 24 条均通过）
- 无需登录，正文游客全开
- 已知限制：无封面。站方封面是 AES 加密字节流（浏览器里靠 `decrypt.worker.js` 解密，类名 `encrypted-image`），App 直接拿 URL 解不了，所以封面规则留空显示默认图

### 一键导入

```
legado://import/bookSource?src=https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fwdfkymd%2Flegado-shuyuan%40main%2Fbanshanren.json
```

手机浏览器打开上面这行，或转成二维码扫码。

### 网络导入

书源管理 → 右上角 ⋮ → 网络导入，粘贴：

```
https://cdn.jsdelivr.net/gh/wdfkymd/legado-shuyuan@main/banshanren.json
```

合一导入（含本站全部源，当前同单源）：

```
https://cdn.jsdelivr.net/gh/wdfkymd/legado-shuyuan@main/all.json
```
