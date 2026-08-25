# fnos-source — yunchui 的飞牛应用源

自建飞牛 fnOS 第三方应用源，当前提供 **Hermes Studio**（Hermes Agent 桌面 / Web 控制台与本地运行时）。

## 使用说明（飞牛应用中心）

1. 打开飞牛 OS 的 **应用中心**
2. 点击 **自定义源** / **添加源**
3. 填入本仓库地址：`https://github.com/yunchui/fnos-source`
4. 应用中心会自动读取 `fnpack.json`（v1）或 `fnpackv2.json`（v2）
5. 找到 **Hermes Studio** 并安装

## 应用列表

| 包名 | 显示名 | 版本 | 平台 | 说明 |
|------|--------|------|------|------|
| hermes-studio | Hermes Studio | 0.6.46-1 | all | 🐴Hermes Agent 本地运行时与 Web 控制台 |

## FPK 下载来源

- 元数据：本仓库 `fnpack.json` / `fnpackv2.json`
- 实际安装包（FPK）：由 [yunchui/Fnos-Hermes-Studio](https://github.com/yunchui/Fnos-Hermes-Studio) 的 GitHub Actions 自动构建并发布

## 结构说明

```
fnos-source/
├── fnpack.json          # 源索引 v1（飞牛应用中心读取）
├── fnpackv2.json        # 源索引 v2（新版飞牛应用中心读取）
└── hermes-studio/        # 应用目录
    ├── ICON.PNG         # 应用图标
    ├── README.md        # 应用说明
    └── Preview/         # 预览图
        └── 1.png
```

## 更新机制

Hermes Studio 的 FPK 由上游自动构建（`build.yml` Gitub Actions）。本源的 `fnpack.json` 下载地址指向其 GitHub Release，FPK 发布后即可获得新版本。
