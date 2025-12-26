# Portfolio Website Checkpoint - 2025-12-24

## Session Summary
취업/이직용 개발자 포트폴리오 웹사이트 구축 및 개선 작업

---

## 완료된 작업

### 1. 프로젝트 구조
```
portfolio/
├── index.html              # 메인 페이지 (9개 프로젝트 카드)
├── about.html              # 소개 페이지 (경력/학력 타임라인)
├── projects/               # 개별 프로젝트 상세 페이지
│   ├── 1bus.html          # 일버스 (견적요청 50% + 기사장터 50%)
│   ├── junggubus.html
│   ├── pt-reports.html
│   ├── junggu-shuttle.html
│   ├── route-builder.html
│   ├── route-optimizer.html
│   ├── hydrogen-infra.html
│   ├── bizno.html
│   └── onbus-platform.html
├── demos/                  # 라이브 데모 파일
│   ├── junggubus-editor.html
│   ├── junggubus-viewer.html
│   ├── hrs-dashboard.html
│   ├── coupang-route.html
│   └── pt-reports/
└── images/projects/        # 프로젝트 상징 이미지 (9개)
    ├── junggubus/main.png
    ├── pt-reports/main.png
    ├── junggu-shuttle/main.png
    ├── route-builder/main.png
    ├── route-optimizer/main.png
    ├── hydrogen/main.png
    ├── 1bus/main.png
    ├── bizno/main.png
    └── onbus/main.png
```

---

### 2. 주요 수정 이력

| 항목 | 변경 전 | 변경 후 |
|------|--------|--------|
| 프로젝트 | AI Rural | 일버스 (1-bus.com) |
| 카드 이미지 | 캡쳐 스크린샷 | 그라데이션 + 텍스트 상징 이미지 |
| 히어로 문구 | "AI 도구로 직접 만들었습니다" | "경험은 깊고, 실행은 빠릅니다." |
| 서브 문구 | - | "26년 경력의 CTO/COO가 전략 구상에서 MVP 실행까지 직접 리드합니다." |
| 다운로드 수치 | 200만+ | 300만+ |

---

### 3. 일버스(1bus.html) 최종 구성

**50:50 믹싱 구조:**
- **견적 요청** (50%): 고객↔사업자 연결, 가격 비교, 투명한 거래
- **기사장터 & 커뮤니티** (50%): 구인/구직, 버스매매, 자유게시판

**UI 구성:**
- 히어로: 흰색 배경 + 로고 이미지 (cdn.imweb.me)
- 2컬럼 카드: 견적요청 | 기사장터
- 기술 스택: 아임웹(노코드), 폼 빌더, 게시판 시스템, SEO

**index.html 카드:**
- 로고 대신 `images/projects/1bus/main.png` 사용 (일관성)
- 설명: "전세버스 종합 플랫폼. 견적 요청, 기사 구인/구직, 버스매매를 노코드로 빠르게 구축."

---

### 4. 기술 스택

- **프론트엔드**: Tailwind CSS (CDN), Pretendard 폰트
- **테마**: 다크 프리미엄 (히어로), 라이트 (카드/컨텐츠)
- **이미지 생성**: Python PIL (그라데이션 + 텍스트)
- **데모**: 정적 HTML (Junggubus, HRS, PT Reports, Coupang)

---

## 프로젝트 인벤토리 (9개)

| # | 프로젝트 | 카테고리 | 데모 | 상태 |
|---|---------|---------|------|------|
| 1 | 내편 중구버스 노선 편집기 | Web App | Editor + Viewer | ✅ |
| 2 | 노선 프레젠테이션 뷰어 | Web App | Demo | ✅ |
| 3 | 중구 셔틀버스 관리 시스템 | Web App | - | ✅ |
| 4 | 쿠팡 FC 노선 빌더 | Web App | Live + Output | ✅ |
| 5 | 3단계 노선 최적화 파이프라인 | Automation | - | ✅ |
| 6 | 수소충전소 분석 대시보드 | Analysis | Dashboard | ✅ |
| 7 | 일버스 (1-bus.com) | Web Platform | Website | ✅ |
| 8 | 계약 관리 자동화 | Analysis | - | ✅ |
| 9 | OnBus 운송 플랫폼 | Platform | - | ✅ |

---

## 최근 세션 수정 (2025-12-24 추가)

### 5. junggu-shuttle.html ASCII 테이블 수정
- **Issue**: System Architecture 다이어그램 정렬 불량
- **Solution**: 박스 크기 일관성, 제목 중앙 정렬, 화살표 라인 정렬, `leading-relaxed` 클래스 추가

### 6. onbus-platform.html 용어 수정
- **Issue**: "마을버스" 용어 오류
- **Solution**: 전체 "마을버스" → "공공버스" 변경 (3곳)
  - "지자체 공공버스 앱"
  - "지자체 공공버스를 위한 아키텍처를 설계했습니다"
  - "공공버스 앱으로 운영되고 있습니다"

---

## 남은 작업

- [ ] Netlify 배포
- [ ] 커스텀 도메인 연결
- [ ] Google Analytics 추가
- [ ] Open Graph 메타태그 최적화
- [ ] 영문 버전 (선택)

---

## 사용자 선호 사항

1. **톤**: 거창한 문구 지양, 실용적/겸손한 톤 선호
2. **관점**: 개발자 X → CTO/COO 관점, 전략+실행력 강조
3. **MVP**: 노코드/빠른 실행력 어필
4. **일관성**: 카드 이미지 스타일 통일

---

## 핵심 파일 경로

```
메인: C:\Users\Phantasmagoria\Desktop\portfolio\index.html
소개: C:\Users\Phantasmagoria\Desktop\portfolio\about.html
일버스: C:\Users\Phantasmagoria\Desktop\portfolio\projects\1bus.html
계획: C:\Users\Phantasmagoria\.claude\plans\jolly-frolicking-reef.md
```
