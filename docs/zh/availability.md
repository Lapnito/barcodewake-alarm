---
title: BarcodeWake 可用性和版本
lang: zh
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# BarcodeWake 可用性和版本

BarcodeWake 在 Android 上有一个经过验证的 Google Play 公开列表。 在审计日期，Google Play 显示版本 1.0.0，而检查的源代码项目声明版本 2.0.0+2。 未验证到公开的 App Store 列表。

## 已验证的公开分发

Android 软件包公开列为 [BarcodeWake: Google Play 上的无作弊闹钟](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us)。 本文档捕获的商店快照报告版本 1.0.0，最后更新日期为 2026 年 3 月。 该快照是列表在某一时间点的证据，并非保证每个地区都看到相同的推广或列表保持不变。

源代码树包含 Android 和 iOS 平台项目。 平台源代码不能证明商店发布。 由于未验证到 App Store 页面，这些文档将 iOS 相关项目描述为仅源代码支持，不告诉读者 BarcodeWake 目前可从 Apple 下载。

## 为什么出现两个版本号

仓库 `pubspec.yaml` 声明源代码版本 2.0.0+2，其更新日志描述了比捕获的公开列表更广泛的任务系统。 商店推广可能落后于开发分支，按地区分阶段进行，或者根本没有发布。 没有匹配的商店记录，安全的说法是狭窄的：能力存在于检查的源代码中，而公开可用性仅对捕获的商店版本有证据。

当功能页面说"当前源代码"时，这个措辞是有意的。 在依赖任务链、设置共享或其他更新功能之前，请检查已安装应用程序的版本和可见控件。 从[任务行为](features/missions.md)开始，然后仅对已安装版本实际显示的选项使用[设置指南](guides/set-up-an-alarm.md)。

## 设备要求和安装检查

扫描需要相机权限。 NFC、运动和步数任务需要相应的设备硬件。 Android 闹钟传递可能需要通知和精确闹钟访问，某些制造商还有其他电池设置。 从经验证的商店列表安装，创建近期的测试闹钟，锁定屏幕，并在依赖它进行重要叫醒之前确认声音和所选任务。

有关简明的边界列表，请阅读[产品事实](facts.md)。 如果测试闹钟失败，请按照[闹钟传递故障排除](help/alarm-delivery.md)进行操作，而不是反复重新创建闹钟。

