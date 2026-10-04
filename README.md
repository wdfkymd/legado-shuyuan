# legado-shuyuan

Legado（阅读 App）书源。

## 搬山人小说网

- 站点：https://www.banshanren.com
- 功能：搜索、详情、目录、正文、发现页（8 个分类，支持翻页）
- 规则已按现站结构实测（搜索/详情/目录 9 章/正文 172 段/发现 24 条均通过）
- 无需登录，正文游客全开

### 一键导入

```
legado://import/bookSource?src=https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fwdfkymd%2Flegado-shuyuan%40v1.1.0%2Fbanshanren.json
```

手机浏览器打开上面这行，或转成二维码扫码。

### 网络导入

书源管理 → 右上角 ⋮ → 网络导入，粘贴：

```
https://cdn.jsdelivr.net/gh/wdfkymd/legado-shuyuan@v1.1.0/banshanren.json
```

合一导入（全部源）：

```
https://cdn.jsdelivr.net/gh/wdfkymd/legado-shuyuan@v1.1.0/all.json
```

## 和图书

- 站点：https://www.hetushu.com
- 功能：搜索、详情、目录（1604 章实测）、正文、发现页（榜单）
- 封面明文直链；正文站方水印已过滤；搜索需 Referer，已内置请求头

### 一键导入

```
legado://import/bookSource?src=https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fwdfkymd%2Flegado-shuyuan%40v1.1.0%2Fhetushu.json
```

### 网络导入

```
https://cdn.jsdelivr.net/gh/wdfkymd/legado-shuyuan@v1.1.0/hetushu.json
```
