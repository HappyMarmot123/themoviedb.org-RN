# Project

### RN + Expo Go App(52ver)

디바이스와 스마트폰의 와이파이를 동일한 것으로 설정하세요.  
터미널 실행명령어: npx expo start --tunnel  
Expo Go 앱 에러발생시: npx expo start --tunnel
Expo Go 앱에서 QR코드를 스캔하세요.

Android apk  
[2024-12-10] ver.1: https://expo.dev/artifacts/eas/8MUmD6kzrrh8tB7Y1DKqcX.apk

## Why use Expo?

Expo는 create-react-native-app을 기반으로 시작할 수 있어, 복잡한 설정 없이 바로 프로젝트를 시작할 수 있습니다.  
React Native에서는 Xcode(iOS)나 Android Studio(Android) 등 설정해야 할 환경이 많지만,  
Expo는 이러한 설정을 생략하고 즉시 앱 개발에 집중할 수 있게 도와줍니다.  
Expo는 개발 서버를 제공하며, **핫 리로드(Hot Reloading)**와 라이브 리로드(Live Reload) 기능을 지원합니다.  
실제 디바이스에서 앱을 실행할 때 코드 변경이 바로 반영되므로, 개발 속도가 빨라집니다.

## Which project did i cloned

- 참조링크1 : https://developers.themoviedb.org/3
- 참조링크2 : https://www.themoviedb.org/
- 참조링크3 : https://play.google.com/store/apps/details?id=uz.isystem.tmdbapp&hl=en_US

## 제약사항 및 코딩과제

### MISSION. The Movie DB APP 클론 코딩하기

| 프레임워크
: React Native
| 개발언어
: Typescript (or Javascript )
| 상태관리
: Redux (or Redux-toolkit)
| 제약상세

- 목록화면이 정상적으로 노출되어야 한다.
- 검색(영화명) 기능이 정상적으로 동작되어야 한다.
- 필터(인기순, 평점수, 신규순, 즐겨찾기) 기능이 정상적으로 동작되어야 한다.
- 상세화면으로 이동하고, 영화정보가 출력되어야 한다.
- 상세화면에서 트레일러 선택시 유튜브앱이 실행되어야 한다.
- 상세화면에서 평점주기 기능이 지원되어야 한다.
- 즐겨찾기 기능이 정상적으로 동작되어야 한다.
  ※ 위 내용을 제외한 사항은 자유롭게 진행해주세요.
  ※ 참조링크3을 휴대폰에 설치하시어 참조하면서 모바일 UI/UX 를 구성해주세요.
  ※ 안드로이드 기준으로 제출해주세요.

## 진행사항

구현(필수사항) - 목록화면, 검색화면, 상세화면, 평점주기, 즐겨찾기, 유투브(웹,앱)영상열기 등  
미구현(필수사항) - 평점주기  
미구현(선택사항) - 카메라, 사진등록

### 버그리스트

[2024-12-05 ~ 2024-12-10]

- ~~홈: 상단 슬라이드 이미지가 브라우저 뷰에서 크기 크래싱 되는 이슈~~
- ~~홈: 'See All Movies' 슬라이드 오른쪽 끝까지 스크롤 후 필터팝업(즐겨찾기) 선택 시 아무것도 안보이는 이슈~~
- ~~홈: 'See All Movies' 이미지 요소의 이미지가 프레임 크기가 아닌 본인 크기를 유지하는 이슈~~
- ~~검색: 브라우저 뷰에서 RN Animated 에러 이슈~~
- ~~검색: 상단 우측 돋보기 UI 이슈~~
- ~~검색: 하단으로 최대 5페이지까지 쭈욱 스크롤 한 후 다시 상단으로 스크롤 할 경우 alert 뜨는 이슈~~
- ~~검색: 검색 목록 클릭 후 스마트폰 디바이스의 '뒤로가기' 버튼 클릭 시 홈으로 가는 이슈 (세팅 필요)~~
- ~~상세: 디바이스 크기에 따른 영화 '장르태그' 슬라이드가 가려지는 이슈~~
- ~~프로필: 로그인 팝업 및 프로필 정상화~~
- 로그인: 로그인 팝업 첫 마운트 시 로그인 버튼 (isValid default value false) 동작 안하는 이슈
- 즐겨찾기: 기능만 구현됬으며 사용자 편의성과 디자인 개선 필요함
- API: api 조회는 빠르지만 이미지 조회 속도 개선 필요함
- 라이브러리: qs 및 lodash 사용하여 코드 개선하기

eas build -p android --profile preview
