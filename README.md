# Loon 规则列表

适用于 **Loon** 的去广告规则集合，基于旧版 Rewrite 语法（`[Rewrite]` + `[Script]`），Loon 3.x 全版本兼容。

## 规则列表

| 应用 | 规则文件 | 依赖脚本 | 状态 |
| --- | --- | --- | --- |
| 菜鸟 | [`CainiaoAds-Loon.conf`](./CainiaoAds-Loon.conf) | `amdc.js`<br>`cainiao_json.js` | ✅ 可用 |
| 网易邮箱大师 | [`NeteaseMailAds-Loon.conf`](./NeteaseMailAds-Loon.conf) | 无 | ✅ 可用 |
| 什么值得买 | [`SmzdmAds-Loon.conf`](./SmzdmAds-Loon.conf) | `smzdm_json.js` | ✅ 可用 |
| 高德地图 | [`AmapAds-Loon.conf`](./AmapAds-Loon.conf) | `amap.js`<br>`amdc.js` | ✅ 可用 |
| 12306 | [`12306-Loon.conf`](./12306-Loon.conf) | `12306.js` | ✅ 可用 |
| 酷安 | [`Coolapk-Loon.conf`](./Coolapk-Loon.conf) | `coolapk.js` | ✅ 可用 |

## 订阅地址

### 菜鸟

```
https://cdn.jsdelivr.net/gh/zzxyscc6699/cainiao-moyu@master/CainiaoAds-Loon.conf
```

### 网易邮箱大师

```
https://cdn.jsdelivr.net/gh/zzxyscc6699/cainiao-moyu@master/NeteaseMailAds-Loon.conf
```

### 什么值得买

```
https://cdn.jsdelivr.net/gh/zzxyscc6699/cainiao-moyu@master/SmzdmAds-Loon.conf
```

### 高德地图

```
https://cdn.jsdelivr.net/gh/zzxyscc6699/cainiao-moyu@master/AmapAds-Loon.conf
```

### 12306

```
https://cdn.jsdelivr.net/gh/zzxyscc6699/cainiao-moyu@master/12306-Loon.conf
```

### 酷安

```
https://cdn.jsdelivr.net/gh/zzxyscc6699/cainiao-moyu@master/Coolapk-Loon.conf
```

## 使用方法

1. Loon → 配置 → 重写 → 右上角 `+` → 引用
2. 粘贴上面对应的订阅地址
3. 开启「重写」与「MitM」
4. 安装并信任 Loon 的 CA 证书

> 证书没装或 MitM 没开，所有 HTTPS 规则都不会生效。

## 说明

- 脚本通过 jsDelivr CDN 加载，不依赖 `raw.githubusercontent.com`，国内可直连。
- 脚本文件需与本仓库规则文件放在同一目录，否则 `script-path` 会 404。
- `12306.js` 目前指向 `ddgksf2013/Scripts`，如需完全自持请自行上传到本仓库并修改 `12306-Loon.conf` 中的地址。
