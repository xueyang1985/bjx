# bjx — TVBox / OK影视 自用接口

## 文件说明

| 文件 | 源数 | 参与搜索 | jar | 适合 |
|---|---|---|---|---|
| `all-mini.json` | 73 | 30 | 3 | 1G 内存盒子，最省 |
| `all-lite.json` | 171 | 38 | 4 | 2G 盒子，推荐 |
| `all-clean.json` | 171 | 125 | 4 | 只要影视，搜索全开 |
| `all.json` | 225 | 167 | 4 | 含网盘/磁力/解析的原始合集 |

全部是 jar 爬虫源（`all.json` 除外），已剔除网盘、磁力、P2P、js 解析、采集接口。

## 配置地址

```
https://ghfast.top/https://raw.githubusercontent.com/xueyang1985/bjx/refs/heads/main/all-mini.json
```

`all-mini.json` 换成 `all-lite.json` / `all-clean.json` / `all.json` 即可切换。

## 直连（不走加速）

把地址里的 `https://ghfast.top/` 去掉：

```
https://raw.githubusercontent.com/xueyang1985/bjx/refs/heads/main/all-mini.json
```

`直连备用/` 目录里是同样换好直连前缀的 4 个 json，需要时直接覆盖根目录那份。

## 注意

- `jar/` 目录下的 4 个 jar 已被 json 用绝对地址引用，**不要改名、不要移动**，删了对应的源就全部打不开。
- 改配置时只要 md5 不变，`spider` 里的地址就不用动；换了 jar 才需要同步改 md5。
- 仓库设成 Private 后 TVBox 读不到 raw，必须保持 Public。
