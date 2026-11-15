# 단골창구 iOS 앱 껍데기 (com.weaveapp.dangol)

- 화면은 https://dangol.org 에서 그대로 불러옵니다(손님 · 사장님 같이 씀). 화면 수정은 dangol.org 쪽만 고치면 됩니다.
- 폴더 없이 파일만 둡니다. Codemagic 이 빌드 때 `npx cap add ios` 로 아이폰 폴더를 만들고 ios_setup.py 가 설정을 끼워 넣습니다.
- AppDelegate.swift 는 가림(aliascall-ios)에서 **알림 · 애플 결제만** 옮긴 작은 판입니다(전화 · 글자 스캐너 없음).
- 결제 상품: 애플 `dangol_1y_nr` (1년 9,900원 · 비갱신 구독) — 화면은 `dangol_1y` 로 부르고 앱이 `_nr` 를 붙입니다.
- 저장소에 넣어야 할 것: `GoogleService-Info.plist` (Firebase 에일리어스콜 프로젝트 → iOS 앱 com.weaveapp.dangol)
