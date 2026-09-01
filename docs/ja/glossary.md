---
title: BarcodeWake 用語集
lang: ja
app: barcodewake-alarm
page_type: glossary
updated: 2026-09-01
targets:
  - BarcodeWake terminology
facts_used:
  - core_measurement
  - data_storage
  - export_formats
---

# BarcodeWake 用語集

BarcodeWakeは、アラームを解除するために必要なアクションを「ミッション」と呼びます。スキャンミッションは登録された物理コードを検証し、チャレンジミッションは解答や動きを検証し、共有とバックアップは異なる交換形式を指します。

## アラームとミッションの用語

- Alarm: 時刻、動作する曜日、音、および解除設定を含むスケジュールされた起床イベント。
- Mission: 解除前に完了する必要があるタスク。
- Scan mission: 登録されたコード表現と照合されるバーコード、QR、またはNFCベースのタスク。
- Challenge mission: 数学、入力、振動、または歩数タスク。
- Single mode: アラームに対して1つの設定済みミッションが実行されます。
- Chain mode: 設定されたミッションが選択された順序で実行されます。
- Random mode: 設定されたセットから1つのミッションが選ばれます。
- Difficulty: タスクの要求を変更するミッション設定です。実際の効果はミッションの種類に依存します。

## データと信頼性に関する用語

- Registered code: スキャン ミッションに関連する物理的なバーコード、QRコード、またはNFCタグ。
- Code hash: 現在のストレージおよび交換パスで登録値の照合に使用される一方向のSHA-256表現。
- Local backup: アプリデータを保存または復元するためのエクスポートされた表現。
- Setup QR: 登録コード、NFC識別子、PIN、履歴を省略した限定的な構成共有フォーマット。
- Reliability Doctor: アラームの配信を妨げる可能性のある権限とシステム設定のためのアプリ内診断です。
- Exact-alarm access: Android システム権限または時間的に重要なスケジューリングを許可するポリシー。
- Battery optimisation: バックグラウンド実行を制限する可能性のあるオペレーティングシステムまたはベンダーの制御。

全機能の関係については、[ミッションとミッション連鎖](features/missions.md) を参照してください。エクスポート形式の違いについては、[バックアップと共有](guides/backup-and-sharing.md) を参照してください。[事実ページ](facts.md) は、アプリが測定しないと主張する内容を定義しています。

