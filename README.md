# KIM SALES — 김 판매·재고관리 시스템

한국 수입 김 상품의 판매, 재고, 커미션을 통합 관리하는 PWA입니다.

## 주요 기능

- 상품(SKU) 관리 — 카테고리별 다품목, 수입처별 분류
- 수입처 관리 — 한국 공급사 정보 관리
- 수입·입고 관리 — 배치별 원가 자동 계산 (KRW→VND 환율 적용)
- 판매처 관리 — 대형유통·도매·소개연결처 구분
- 소개자·커미션 관리 — 개당 고정 커미션, 미지급 추적
- 판매가 관리 — 자유 변경 + 전체 이력 보존
- 판매 등록 — FIFO 자동 재고 차감, 커미션 자동 계산
- 재고 현황 — 배치별 추적, 유통기한 임박 알림
- 수익 분석 — 실수령 기준 손익, 외상 관리
- 대시보드 — 오늘의 매출, 알림 통합 표시

## 설치 (GitHub Pages)

1. GitHub에 `kim-sales` 저장소 생성
2. 이 폴더의 모든 파일을 업로드
3. Settings → Pages → Source: main branch, /root
4. 생성된 URL로 접속
5. Firebase 설정 입력

## Firebase 설정

Firebase Console → 프로젝트 설정 → 앱 → SDK 설정에서:
- `apiKey`
- `authDomain`
- `databaseURL`
- `projectId`

위 4가지 값을 앱 최초 실행 시 입력합니다.

### Firebase Realtime Database 보안 규칙 (3명 관리자용)

```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
```

> 운영 환경에서는 Firebase Authentication 연동 후 규칙을 강화하세요.

## 언어 지원

한국어 / Tiếng Việt (좌측 하단 언어 전환)
