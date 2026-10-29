# legado-shuyuan

Legado（阅读 App）书源。

## 网络导入

书源管理 → 右上角 ⋮ → 网络导入，粘贴：

**搬山人小说网：**
```
https://cdn.jsdelivr.net/gh/wdfkymd/legado-shuyuan@v1.5.1/banshanren.json
```

**爱丽丝书屋：**
```
https://cdn.jsdelivr.net/gh/wdfkymd/legado-shuyuan@v1.5.1/alicesw.json
```

**Pixiv 小说：**（仅主分支，v1.5.1 标签里还没有）
```
https://cdn.jsdelivr.net/gh/wdfkymd/legado-shuyuan@main/pixiv.json
```

**合一导入（全部源）：**
```
https://cdn.jsdelivr.net/gh/wdfkymd/legado-shuyuan@v1.5.1/all.json
```

---

## 搬山人小说网

- 站点：https://www.banshanren.com
- 功能：搜索、详情、目录、正文、发现页（8 个分类，支持翻页）
- 规则已按现站结构实测（搜索/详情/目录 9 章/正文 172 段/发现 24 条均通过）
- 无需登录，正文游客全开

### 一键导入

```
legado://import/bookSource?src=https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fwdfkymd%2Flegado-shuyuan%40v1.5.1%2Fbanshanren.json
```

手机浏览器打开上面这行，或转成二维码扫码。

## 爱丽丝书屋

- 站点：https://www.alicesw.com（发布页：https://alicesw.click/，入口可能更换）
- 功能：搜索（精确命中《神秘复苏》原书，1610 章）、详情（封面明文）、目录（单页全量正序）、正文、发现页（最新/人气/字数排行带翻页）
- 搜索页无封面（站方列表纯文字）；详情页封面简介全有；站方地域拦只针对美国机房，无影响

### 一键导入

```
legado://import/bookSource?src=https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fwdfkymd%2Flegado-shuyuan%40v1.5.1%2Falicesw.json
```

## Pixiv 小说

- 站点：https://www.pixiv.net/novel
- 功能：搜索（单篇 + 系列，系列结果自动按系列成书；搜作者时在作者名前加 `@`，如 `@蘑菇麵要加蛋`，先查作者 ID 再取作者全部作品，查不到作者时回落到标签搜索；不加前缀按标签搜，直接打作者名不加 `@` 只会命中打了这个标签的作品）、详情（简介取 caption || description，字数取 textCount，不再依赖 init 结果）、目录（系列用 content_titles 全量标题列表，单篇只有 1 章）、正文
- 必须登录：导入后在书源管理里打开本源登录 pixiv 账号，登录态存在 Cookie 里；未登录时 pixiv ajax 接口直接报错
- 规则已在本机按 Legado @js 求值对测试数据跑通（标签搜 1 条、作者搜 2 条（系列 + 单篇，系列内单篇已去重）、详情简介/字数/系列目录、正文均通过），但本机机房 IP 直连 pixiv ajax 全是 403，真站数据尚未在本机拉通，手机上家用网络 + 登录 Cookie 后再实测作者搜的真站返回结构
- 暂无发现页；正文内嵌插图 [pixivimage:xxx] 只按原文文本显示，不转图片；R18 只在账号本身有权限时可见

### 一键导入

```
legado://import/bookSource?src=https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fwdfkymd%2Flegado-shuyuan%40main%2Fpixiv.json
```

手机浏览器打开上面这行，或转成二维码扫码。
