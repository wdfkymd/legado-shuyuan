# legado-shuyuan

Legado（阅读 App）书源。

## 搬山人小说网

- 站点：https://www.banshanren.com
- 功能：搜索、详情、目录、正文、发现页（8 个分类，支持翻页）
- 规则已按现站结构实测（搜索/详情/目录 9 章/正文 172 段/发现 24 条均通过）
- 无需登录，正文游客全开

### 一键导入

```
legado://import/bookSource?src=https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fwdfkymd%2Flegado-shuyuan%40v1.4.0%2Fbanshanren.json
```

手机浏览器打开上面这行，或转成二维码扫码。

### 网络导入

书源管理 → 右上角 ⋮ → 网络导入，粘贴：

```
https://cdn.jsdelivr.net/gh/wdfkymd/legado-shuyuan@v1.4.0/banshanren.json
```

合一导入（全部源）：

```
https://cdn.jsdelivr.net/gh/wdfkymd/legado-shuyuan@v1.4.0/all.json
```

## 笔趣阁（推荐）

- 站点：https://m.bqge.cc
- 功能：搜索（POST，精确命中《神秘复苏》原书）、详情、目录（1596 章，32 页自动翻页实测收敛）、正文（长章节自动拼页，水印已过滤）、发现页（7 个分类带翻页）
- 搜索页、详情页封面简介全有；UTF-8 无盾直连

### 一键导入

```
legado://import/bookSource?src=https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fwdfkymd%2Flegado-shuyuan%40v1.4.0%2Fbiquge.json
```

### 网络导入

```
https://cdn.jsdelivr.net/gh/wdfkymd/legado-shuyuan@v1.4.0/biquge.json
```
