---
title: BarcodeWake 文件
lang: zh_Hant
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake 文件

BarcodeWake 是一款鬧鐘應用程式，它將關閉鬧鐘變成一個刻意的行為。鬧鐘可以要求掃描已儲存的條碼或 QR 碼、一個簡短的認知任務、搖晃序列或步數目標，而不是僅依賴於螢幕上的一個簡單按鈕。

## BarcodeWake 的與眾不同之處

核心概念是距離加上意圖。如果註冊的程式碼附著在遠離床鋪的物品上，關閉鬧鐘就意味著起床、走到那個物品並掃描它。相同的鬧鐘模式也可以使用數學、打字、搖晃或步數任務。目前的原始碼支援單一任務、按順序鏈接或從已配置的任務中隨機選擇。

這種阻力對於那些在不完全清醒的狀態下關閉普通鬧鐘的人來說很有幫助。這不是睡眠階段分析、醫療指導，也不是確保某人會醒來的保證。硬體支援、權限和供應商的電池控制仍然會影響鬧鐘的傳遞。[任務參考](features/missions.md) 解釋了各種選擇，而[鬧鐘傳遞故障排除](help/alarm-delivery.md) 涵蓋了可能干擾的系統設定。

## 從正確的文件開始

建立鬧鐘並註冊實體程式碼時，使用[設定指南](guides/set-up-an-alarm.md)。在移動資料或傳送設定 QR 碼給其他人之前，請閱讀[備份與分享](guides/backup-and-sharing.md)。分享格式特意排除已註冊的程式碼、NFC 識別碼、PIN 和鬧鐘歷史，因此接收者必須在本地完成敏感設定。

如需簡短、可稽核的摘要，請參閱[產品事實](facts.md)。如需發布狀態，請使用[可用性](availability.md)：本次審計捕獲的公開 Google Play 版本與所檢查原始碼樹中宣告的版本不同。因此，新版原始碼被記錄為原始碼功能，而非作為已發布的商店版本。

## 隱私和可靠性界限

核心設定和任務資料儲存在設備上，無需 BarcodeWake 帳戶。目前的程式碼路徑使用 SHA-256 雜湊值來表示已註冊的程式碼值。可選的遙測功能在隱私權政策中描述為預設停用。這些聲明並不意味著每支手機都會以相同方式傳遞鬧鐘；Android 供應商和作業系統權限仍然可以限制背景行為。

如需了解本地資料處理和作業系統傳遞之間的區別，請閱讀[隱私和可靠性](features/privacy-and-reliability.md)。[標準鬧鐘比較](comparisons/standard-alarm.md) 有助於判斷基於任務的關閉方式是否符合您的起床方式。

