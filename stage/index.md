# 平台愿景

## CLI 简化 DevOps 生命周期

`qtcloud-devops` 的目标是用命令行工具简化 DevOps 生命周期的每个环节。

```
plan     → qtcloud-devops plan       ✅ doctor / edit / status / clean / audit
code     → qtcloud-devops code       ✅ status / audit
build    → qtcloud-devops build      ✅ status / clean / audit
test     → qtcloud-devops test       ✅ status / audit
release  → qtcloud-devops release    ✅ status / audit / publish
deploy   → qtcloud-devops deploy     （待实现）
operate  → qtcloud-devops operate    （待实现）
monitor  → qtcloud-devops monitor    （待实现）
```

每个阶段一页命令参考（`docs/handbook/stage/`），格式统一：

```
操作前检查 → 执行操作 → 操作后验证
```

手册不讲通用知识，只展示 CLI 如何简化该环节的管理。
