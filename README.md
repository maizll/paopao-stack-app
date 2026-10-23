# 泡泡栈 App 更新仓

存放 Android 客户端发布包与版本清单，供官网/API 推送应用内更新。

## 用法

1. 打好 APK 后，在本仓打 [Release](https://github.com/maizll/paopao-stack-app/releases)，资源文件上传 `paopao-stack-x.y.z.apk`。
2. 更新根目录 `latest.json`（见下方字段），提交到 `main`。
3. 运营后台「系统」里也可覆盖：版本名、版本号、APK 直链、更新说明、是否强制。

## `latest.json`

```json
{
  "latestVersion": "1.0.8",
  "versionCode": 108,
  "forceUpdate": false,
  "downloadUrl": "https://github.com/maizll/paopao-stack-app/releases/download/v1.0.8/paopao-stack-1.0.8.apk",
  "changelog": "更新说明"
}
```

当前演示：接口未单独配置时，服务端默认返回 1.0.8，下载地址可先指向站点 `public/` 下的直链或本仓 Release。
