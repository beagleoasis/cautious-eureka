# 증권사 OPEN API를 이용한 자동 매수/매도 서비스 

## 1. 프로젝트 : Rich Beagle
* 증권사 커뮤니티 기능을 이용한 주식 자동 매수/매도 서비스

## 2. 구성
* 안드로이드 App(Kotlin)
  * 나의 매수 금액 관리
  * 잔고 조회 관리
  * 안전 매도 모드 관리
  * 손익 조회 관리
  * 팔로우 유저 관리
  * 거래 관리
  * 수동 주문
  * 보유 주식 조건 주문
* 텔레그램
  * 안드로이드 App의 요청 수신, 플라스크 서버로 전송
* 파이썬 서버(Flask)
  * Notification REST API 서버
  * Scheduler
  * Telegram Message Reader
 
## 3. 대표 기능 
* Telegram 서버
* 자체 제작 한국투자증권 OpenAPI 라이브러리
* 방어 로직
  * 안전 매도
  * 투자금 대비 비율 보정

## 4. 트러블 슈팅
* REST API & Scheduler 간 동시성 문제
* 안드로이드 알림 MQ

