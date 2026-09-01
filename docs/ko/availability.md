---
title: BarcodeWake 가용성 및 버전
lang: ko
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# BarcodeWake 가용성 및 버전

BarcodeWake는 확인된 공개 Google Play 목록이 있는 Android용 앱입니다. 감사 날짜 기준, Google Play에는 버전 1.0.0이 표시되었으며, 확인된 소스 프로젝트는 버전 2.0.0+2를 선언했습니다. 공개 App Store 목록은 확인되지 않았습니다.

## 확인된 공개 배포

Android 패키지는 [Google Play의 BarcodeWake: No Cheat Alarm](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us)으로 공개 목록에 등록되어 있습니다. 이 문서를 위해 캡처된 스토어 스냅샷에는 버전 1.0.0과 2026년 3월의 최종 업데이트 날짜가 보고되었습니다. 해당 스냅샷은 특정 시점의 목록 증거이지, 모든 지역이 동일한 롤아웃을 보거나 목록이 변경되지 않을 것이라는 보장은 아닙니다.

소스 트리에는 Android와 iOS 플랫폼 프로젝트가 포함되어 있습니다. 플랫폼 소스가 스토어 게시를 증명하지는 않습니다. App Store 페이지가 확인되지 않았으므로, 이 문서는 iOS 관련 항목을 소스 지원으로만 설명하며 독자에게 BarcodeWake가 현재 Apple에서 다운로드 가능하다고 알리지 않습니다.

## 두 가지 버전 번호가 나타나는 이유

저장소 `pubspec.yaml`은 소스 버전 2.0.0+2를 선언하며 해당 변경 로그에는 캡처된 공개 목록보다 더 넓은 미션 시스템이 설명되어 있습니다. 스토어 롤아웃은 개발 브랜치보다 지연되거나, 지역별로 스테이징되거나, 단순히 게시되지 않았을 수 있습니다. 일치하는 스토어 기록이 없으면 안전한 설명은 다음과 같습니다: 해당 기능은 확인된 소스에 존재하지만, 공개 가용성은 캡처된 스토어 버전 대해서만 입증됩니다.

기능 페이지에서 "현재 소스"라고 명시하는 경우, 그 표현은 의도적인 것입니다. 미션 체인, 설정 공유 또는 다른 최신 기능에 의존하기 전에, 설치된 앱의 버전과 표시되는 컨트롤을 확인하세요. [미션 동작](features/missions.md)에서 시작한 후, 설치된 빌드가 실제로 표시하는 옵션에 대해서만 [설정 가이드](guides/set-up-an-alarm.md)를 사용하세요.

## 기기 요구사항 및 설치 확인

스캔에는 카메라 권한이 필요합니다. NFC, 모션 및 걸음 수 미션에는 해당하는 기기 하드웨어가 필요합니다. Android 알람 전달은 알림 및 정밀 알람 액세스를 요구할 수 있으며, 일부 제조업체에서는 추가 배터리 설정이 필요합니다. 확인된 스토어 목록에서 설치하고, 단기 테스트 알람을 만든 후, 화면을 잠그고 중요한 기상용으로 의존하기 전에 소리와 선택한 미션 둘 다를 확인하세요.

간결한 범위 목록은 [제품 사실](facts.md)을 읽으세요. 테스트 알람이 실패하면 알람을 반복적으로 다시 만들지 말고 [알람 전달 문제 해결](help/alarm-delivery.md)을 따르세요.

