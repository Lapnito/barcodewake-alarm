---
title: BarcodeWake 文档
lang: zh
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake 文档

BarcodeWake 是一个闹钟，它使关闭闹钟成为一种有意的行为。一个闹钟可以要求扫描已保存的条形码或二维码、一个简短的认知任务、摇晃序列或步数目标，而不是仅仅依赖屏幕上容易按到的按钮。

## 是什么让 BarcodeWake 与众不同

核心思想是距离加上意图。如果注册的代码绑定在远离床的物品上，那么要关闭闹钟就意味着要起身、够到那个物品并扫描它。同样的闹钟模式也可以使用数学题、打字、摇晃或步数任务。当前的源代码支持单一任务、按顺序链接的任务链，或从配置的任务中随机选择。

这种摩擦对于那些会不经意间关闭普通闹钟但没有完全清醒的人来说是有用的。它不是睡眠阶段分析、医疗指导，也不能保证有人一定会醒来。硬件支持、权限和厂商的电池控制仍然会影响闹钟的送达。[任务参考](features/missions.md)解释了各种选择，而[闹钟送达故障排除](help/alarm-delivery.md)涵盖了可能干扰的系统设置。

## 从合适的文档开始

创建闹钟并注册物理代码时使用[设置指南](guides/set-up-an-alarm.md)。在迁移数据或向他人发送设置二维码之前阅读[备份和分享](guides/backup-and-sharing.md)。分享格式特意排除了已注册的代码、NFC 标识符、PIN 码和闹钟历史，因此接收者必须在本地完成敏感信息的设置。

要获取简短、可审计的摘要，请参阅[产品事实](facts.md)。要了解发布状态，请使用[可用性](availability.md)：公开的 Google Play 版本与本次审计所检查的源代码树声明的版本不同。因此，较新的源代码版本被记录为源代码能力，而非作为已发布的商店版本。

## 隐私和可靠性边界

核心配置和任务数据存储在设备上，无需 BarcodeWake 账户。当前代码路径使用 SHA-256 哈希值来表示注册的代码值。可选的遥测数据在隐私政策中被描述为默认禁用。这些声明并不意味着每部手机都会以相同方式送达闹钟；Android 厂商和操作系统权限仍然可能限制后台行为。

阅读[隐私和可靠性](features/privacy-and-reliability.md)了解本地数据处理和操作系统送达之间的区别。[标准闹钟比较](comparisons/standard-alarm.md)有助于决定基于任务的关闭方式是否适合你的起床方式。

