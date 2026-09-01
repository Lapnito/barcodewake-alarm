---
title: BarcodeWake 可用性和版本
lang: zh_Hant
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

BarcodeWake 在 Android 上有已驗證的公開 Google Play 列表。在審計日期，Google Play 顯示版本 1.0.0，而檢查的來源專案宣告版本 2.0.0+2。沒有驗證到公開的 App Store 列表。

## 已驗證的公開分發

Android 套件公開列為 [BarcodeWake: No Cheat Alarm on Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us)。為本文檔捕獲的商店快照報告版本 1.0.0，最後更新日期為 2026 年 3 月。該快照是列表在某個時間點的證據，而不是保證每個地區看到相同的推出或列表保持不變。

來源樹包含 Android 和 iOS 平台專案。平台來源不能證明商店發布。由於沒有驗證 App Store 頁面，這些文件將 iOS 相關項目描述為僅來源支援，不會告訴讀者 BarcodeWake 目前可從 Apple 下載。

## 為什麼會出現兩個版本號

儲存庫 `pubspec.yaml` 宣告來源版本 2.0.0+2，其更新日誌描述了比捕獲的公開列表更廣泛的任務系統。商店推出可能落後於開發分支，按地區分階段推出，或者根本沒有發布。沒有匹配的商店記錄，安全的聲明是狹窄的：功能存在於檢查的來源中，而公開可用性僅針對捕獲的商店版本進行了證明。

當功能頁面說「當前來源」時，這個措辭是經過考慮的。在依賴任務鏈、設定共享或其他較新功能之前，請檢查已安裝應用程式的版本和可見控制項。從 [任務行為](features/missions.md) 開始，然後僅對已安裝版本實際顯示的選項使用 [設定指南](guides/set-up-an-alarm.md)。

## 裝置需求和安裝檢查

掃描需要相機權限。NFC、運動和步數任務需要相應的裝置硬體。Android 鬧鐘傳遞可能需要通知和精確鬧鐘存取，某些製造商還需要額外的電池設定。從已驗證的商店列表安裝，建立短期測試鬧鐘，鎖定螢幕並確認聲音和選擇的任務，然後再依靠它來進行重要的喚醒。

如需簡潔的邊界列表，請閱讀 [產品事實](facts.md)。如果測試鬧鐘失敗，請遵循 [鬧鐘傳遞故障排除](help/alarm-delivery.md)，而不是反覆重新建立鬧鐘。

