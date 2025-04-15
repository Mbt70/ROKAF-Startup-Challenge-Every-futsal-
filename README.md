# ROKAF-Startup-Challenge-Every-futsal-


구성 계획:
1. 서비스 개요 - 간단한 소개
2. 시스템 작동 원리 - 단계별 설명
3. 핵심 기술 요소 설명
4. 사용자 경험 흐름
5. 기대 효과 및 비즈니스 가치

각 섹션은 간결하고 명확하게 작성하며, 비유나 예시를 활용해 이해하기 쉽게 만들겠습니다.

# 풋살 AI 분석 시스템: 경기부터 하이라이트까지

## 1. 한눈에 보는 서비스 개요

**풋살 AI 분석 시스템**은 아마추어 풋살 선수들에게 프로급 경기 분석과 개인 맞춤형 하이라이트를 제공하는 혁신적인 서비스입니다. 풋살장에 설치된 카메라가 경기를 촬영하고, AI가 자동으로 분석하여 개인 및 팀 하이라이트와 상세 지표를 제공합니다.

**주요 기능:**
- 📹 다각도 경기 촬영 (180° 메인 + 보조 앵글)
- 🎯 AI 기반 개인/팀 하이라이트 자동 생성
- 📊 20+ 개인 성과 지표 분석
- 📱 모바일 앱으로 언제 어디서나 접근

## 2. 어떻게 작동하나요? - 5단계 시스템 흐름

### 1️⃣ 경기 촬영 단계
- **스마트 카메라 시스템**이 경기장 전체를 커버
  - Veo Cam 3: 180° 메인 카메라 (AI 자동 트래킹)
  - GoPro x2: 골대 후방 및 사이드 앵글 (역동적 장면 캡처)
- **엣지 컴퓨팅 기술**로 현장에서 1차 처리
  - 영상 압축 및 실시간 스트리밍
  - 네트워크 불안정 시 자동 버퍼링 및 동기화

### 2️⃣ 클라우드 전송 단계
- **안전한 스트리밍 프로토콜**로 AWS 클라우드로 전송
- **멀티 소스 트랜스코딩**으로 다양한 각도 영상 동기화
- **고성능 GPU 서버**에서 실시간 처리 준비

### 3️⃣ AI 분석 단계
- **3D CNN + LSTM 기술**로 행동 및 이벤트 인식
  - 3D CNN: 영상의 공간적 특징 추출 (누가, 어디서, 무엇을)
  - LSTM: 시간적 컨텍스트 분석 (언제, 어떤 순서로, 얼마나 중요한지)
- **컴퓨터 비전 기술**로 선수와 공 추적
  - 선수별 움직임 패턴 분석
  - 실시간 위치 및 속도 측정
- **멀티모달 분석**으로 중요 순간 포착
  - 영상 + 오디오 통합 분석
  - 골, 슛, 패스 등 주요 이벤트 자동 감지

### 4️⃣ 콘텐츠 생성 단계
- **하이라이트 자동 생성**
  - 중요도 점수 기반 장면 선택 (골: 10점, 슛온골: 7점, 좋은 패스: 5점)
  - 이벤트 전후 컨텍스트 포함 클립 생성
  - 멀티앵글 자동 편집
- **개인 및 팀 지표 시각화**
  - 히트맵, 패스 네트워크, 성과 그래프 자동 생성
  - 직관적 인포그래픽으로 복잡한 데이터 시각화

### 5️⃣ 사용자 경험 단계
- **모바일 앱**으로 언제 어디서나 접근
  - 개인 대시보드: 나만의 경기 분석 및 하이라이트
  - 팀 대시보드: 팀 성과 및 전술 분석
- **소셜 공유 기능**으로 하이라이트 즉시 공유
- **성장 추적**으로 경기별 발전 과정 확인

## 3. 핵심 기술: "보이지 않는 코치" AI

### 하이라이트 감지 기술
**AI가 경기의 모든 순간을 지켜보며 중요한 장면을 자동으로 포착합니다**

![하이라이트 생성 프로세스]

1. **이벤트 감지**: 3D CNN + LSTM 모델이 골, 슛, 드리블 등 주요 액션 식별
2. **중요도 평가**: 각 이벤트에 점수 부여 (상황, 난이도, 희귀성 고려)
3. **컨텍스트 분석**: 단순 순간이 아닌 전후 맥락까지 고려
4. **최적 앵글 선택**: 여러 카메라 중 최적의 시청 각도 자동 선택
5. **하이라이트 제작**: 자연스러운 전환과 편집으로 완성도 높은 클립 생성

### 개인 성과 분석 기술
**AI가 선수 한 명 한 명을 세밀하게 분석하여 객관적인 성과 지표를 제공합니다**

1. **선수 식별 및 추적**: 유니폼 색상/번호로 선수 개별 추적
2. **움직임 분석**: 이동 거리, 스프린트, 가속 패턴 측정
3. **기술 분석**: 패스, 슛, 드리블 성공률 계산
4. **포지셔닝 분석**: 공간 점유 및 전술적 위치 평가
5. **종합 평가**: 다차원 지표를 통합한 성과 스코어 제공

### 팀 전술 분석 기술
**팀의 전체 움직임과 연결성을 분석하여 전술적 인사이트를 제공합니다**

1. **패스 네트워크**: 선수 간 연결 패턴 시각화
2. **압박 분석**: 수비 강도 및 효율성 측정
3. **공격 패턴**: 주요 공격 루트 및 전술 파악
4. **공간 활용**: 팀의 공간 점유 및 활용도 분석
5. **시간적 변화**: 체력 저하에 따른 전술 변화 감지

## 4. 실제 서비스 이용 흐름

### 예약부터 분석까지
1. **앱에서 풋살장 예약** - 날짜/시간 선택 및 팀원 등록
2. **경기 진행** - 설치된 카메라가 자동으로 녹화 시작
3. **실시간 알림** - 골 등 중요 이벤트 발생 시 앱으로 즉시 알림
4. **경기 후 분석** - 경기 종료 후 30분 내 기본 하이라이트 제공
5. **상세 분석** - 1시간 내 개인 및 팀 상세 분석 데이터 제공

### 앱 내 주요 화면
- **홈 대시보드**: 최근 경기 하이라이트 및 주요 지표 요약
- **내 하이라이트**: 개인별 베스트 플레이 모음
- **성과 분석**: 상세 지표 및 경기별 성장 트렌드
- **팀 분석**: 팀 전술 및 성과 분석 대시보드
- **경기 갤러리**: 전체 경기 아카이브 및 하이라이트

## 5. 기대 효과 및 차별점

### 사용자 가치
- **객관적 성장 피드백**: "느낌"이 아닌 데이터 기반 피드백
- **시간 절약**: 2시간 경기에서 핵심 장면만 3분으로 압축
- **모티베이션 증가**: 자신의 활약 장면 확인으로 동기부여
- **팀 전술 이해**: 전체 경기 흐름과 팀 전술 파악 용이

### 기술적 차별점
- **풋살 특화 AI**: 11인제 축구가 아닌 풋살에 최적화된 분석
- **멀티모달 분석**: 영상+오디오 통합 분석으로 정확도 향상
- **엣지-클라우드 하이브리드**: 현장 처리와 클라우드 분석 결합으로 안정성 확보
- **개인화 알고리즘**: 사용자 피드백 기반 지속적 개선

### 비즈니스 모델  ->수정필요
- **풋살장 월 구독**: 풋살장당 100-150만원/월
- **개인 구독**: 월 5천원 (프리미엄 분석 및 하이라이트)
- **경기당 결제**: 경기당 2만원 (기본 서비스)
- **확장 가능성**: 리그/대회 운영, 코칭 연계, 교육 콘텐츠

## 6. 구현 로드맵

**MVP 단계 (2-3개월)**
- 기본 카메라 설정 및 스트리밍 인프라
- 골/슛 기본 감지 및 하이라이트 생성
- 핵심 지표 5-7개 구현

**베타 서비스 (3-4개월)**
- 3D CNN + LSTM 모델 고도화
- 완전한 하이라이트 자동 생성
- 20+ 개인 지표 및 팀 분석 구현

**정식 서비스 (6개월)**
- 모든 기능 최적화 및 안정화
- 서울 주요 풋살장 10곳 시범 서비스
- 피드백 기반 지속적 개선

## 시스템 파이프라인
```mermaid
flowchart TD
    %% 메인 섹션
    subgraph CS["📹 데이터 수집 시스템"]
        VC[Veo Cam 3<br>메인 카메라] --> ES
        GP[GoPro x2<br>보조 카메라] --> ES
        ES[엣지 서버] --> |영상 압축 & 버퍼링|KV
        ES --> |네트워크 중단 시|LS[로컬 스토리지]
        LS --> |재연결 후 동기화|KV
    end

    subgraph CL["☁️ AWS 클라우드 인프라"]
        KV[Kinesis Video<br>Streams] --> |실시간 스트리밍|ML[MediaLive]
        ML --> |트랜스코딩|S3R[S3 Raw<br>원본 영상 저장]
        ML --> |영상 처리|EC2
        
        subgraph AIP["🧠 AI 분석 파이프라인"]
            EC2[EC2/ECS<br>GPU 인스턴스] --> OD[객체 감지 & 추적<br>YOLOv8/ByteTrack]
            OD --> |선수/공 위치 데이터|AR[행동 인식<br>3D CNN + LSTM]
            AR --> |행동 분류|ED[이벤트 감지<br>멀티모달 분석]
            ED --> |중요도 점수화|HL[하이라이트 선정]
            
            OD --> |위치 데이터|MA[움직임 분석]
            MA --> |히트맵/거리 계산|PM[성과 지표 모델]
            AR --> |기술 분류|PM
            
            HL --> |중요 장면 선정|MC[MediaConvert]
            PM --> |지표 계산|DB[(DynamoDB/RDS)]
        end
        
        MC --> |하이라이트 클립 생성|S3C[S3 Content<br>가공 콘텐츠 저장]
        DB --> |API 제공|AG[API Gateway<br>AppSync]
        S3C --> |콘텐츠 전송|CF[CloudFront CDN]
    end

    subgraph US["📱 사용자 서비스"]
        CF --> |영상 콘텐츠|AP[모바일 앱]
        AG --> |데이터 & 분석|AP
        
        AP --> |개인 하이라이트|PH[개인 하이라이트<br>& 성과 대시보드]
        AP --> |팀 분석|TA[팀 분석<br>& 하이라이트]
        AP --> |경기 데이터|MD[경기 데이터<br>& 통계]
        
        PH --> |공유|SM[소셜 미디어<br>공유]
        TA --> |저장|HP[하이라이트<br>갤러리]
        MD --> |추적|PT[성과 추적<br>& 개선 제안]
    end

    %% 시스템 간 연결
    CS --> CL
    CL --> US
    
    %% 피드백 루프
    US --> |사용자 피드백|AIP
    
    %% 스타일링 (가독성이 좋도록 진한 배경, 흰색 텍스트)
    classDef camera fill:#D32F2F,stroke:#fff,stroke-width:1px, color:#fff
    classDef edge fill:#757575,stroke:#fff,stroke-width:1px, color:#fff
    classDef cloud fill:#1976D2,stroke:#fff,stroke-width:1px, color:#fff
    classDef ai fill:#7B1FA2,stroke:#fff,stroke-width:1px, color:#fff
    classDef storage fill:#388E3C,stroke:#fff,stroke-width:1px, color:#fff
    classDef content fill:#FBC02D,stroke:#fff,stroke-width:1px, color:#fff
    classDef app fill:#F57C00,stroke:#fff,stroke-width:1px, color:#fff
    classDef delivery fill:#E64A19,stroke:#fff,stroke-width:1px, color:#fff
    
    class VC,GP camera
    class ES,LS edge
    class KV,ML,EC2,AG,CF cloud
    class OD,AR,ED,HL,MA,PM ai
    class S3R,S3C,DB storage
    class MC content
    class AP,PH,TA,MD appapp
    class SM,HP,PT delivery
```



## 시스템 상세 파이프라인

```mermaid
flowchart TD
    %% 메인 섹션 - 데이터 수집
    subgraph CAPTURE["1️⃣ 경기 데이터 수집"]
        direction TB
        V[Veo Cam 3<br>180° 메인 카메라] --> |자동 트래킹| EDGE
        G1[GoPro Hero 13<br>골대 후방 각도] --> EDGE
        G2[GoPro Hero 13<br>사이드 각도] --> EDGE
        
        subgraph EDGE["엣지 컴퓨팅 (현장 처리)"]
            EP[영상 전처리<br>압축 및 동기화] --> BF[스트리밍 버퍼]
            BF --> |안정적 네트워크| ST[RTMP/HLS 스트리밍]
            BF --> |네트워크 불안정| LS[로컬 저장<br>및 재전송 메커니즘]
            LS --> |네트워크 복구 후| ST
        end
    end

    %% 클라우드 처리
    subgraph CLOUD["2️⃣ AWS 클라우드 처리"]
        direction TB
        KVS[Kinesis Video<br>Streams] --> |실시간 수신| ML[MediaLive<br>트랜스코딩]
        ML --> |포맷 변환| S3R[S3 Raw Storage<br>원본 영상]
        ML --> |분석용 스트림| COMPUTE
        
        subgraph COMPUTE["컴퓨팅 리소스"]
            EC2[EC2 g4dn/g5<br>GPU 인스턴스] --> |실시간 처리| ECS[ECS/EKS<br>컨테이너 오케스트레이션]
            EC2 --> |배치 처리| BATCH[AWS Batch<br>대규모 병렬 처리]
        end
    end

    %% AI 분석 파이프라인
    subgraph AI["3️⃣ AI 분석 파이프라인"]
        direction TB
        subgraph CV["컴퓨터 비전 모듈"]
            OD[객체 감지<br>YOLOv8] --> TR[객체 추적<br>ByteTrack/DeepSORT]
            TR --> |선수/공 위치 데이터| CM[코트 매핑<br>호모그래피 변환]
        end
        
        subgraph ACT["행동 인식 모듈"]
            C3D[3D CNN<br>I3D 아키텍처] --> |시공간 특징| LSTM[Bi-directional LSTM<br>시퀀스 모델링]
            POSE[포즈 추정<br>OpenPose] --> |자세 분석| ACTION[행동 분류기<br>패스/슛/태클/드리블]
        end
        
        subgraph EVENT["이벤트 감지 모듈"]
            MULTI[멀티모달 분석<br>영상+오디오] --> |이벤트 감지| SCORE[중요도 점수화<br>알고리즘]
            RULE[규칙 기반 시스템<br>골/위험 찬스] --> SCORE
            SCORE --> |임계값 필터링| HILIGHT[하이라이트 후보<br>선정]
        end
        
        subgraph METRIC["지표 계산 모듈"]
            MOVE[움직임 분석<br>거리/속도/가속] --> |물리적 지표| PLAYER[선수 성과 모델]
            ACTION --> |기술적 지표| PLAYER
            POS[포지셔닝 분석<br>공간 점유] --> |전술적 지표| PLAYER
            PLAYER --> |개인 지표| STATS[통계 엔진]
            PLAYER --> |팀 집계| TEAM[팀 성과 모델]
            TEAM --> |팀 지표| STATS
        end
        
        CV --> ACT
        CV --> EVENT
        CV --> METRIC
        ACT --> EVENT
    end

    %% 콘텐츠 생성
    subgraph CONTENT["4️⃣ 콘텐츠 생성"]
        direction TB
        HILIGHT --> |중요 장면 선택| CLIP[클립 생성기<br>AWS MediaConvert]
        CLIP --> |개인별 하이라이트| PERS[개인 하이라이트<br>패키지]
        CLIP --> |팀 하이라이트| TEAM_H[팀 하이라이트<br>패키지]
        CLIP --> |전체 경기 하이라이트| GAME_H[경기 하이라이트<br>패키지]
        
        STATS --> |데이터 가공| VIZ[데이터 시각화<br>엔진]
        VIZ --> |히트맵| HEAT[히트맵<br>시각화]
        VIZ --> |패스 네트워크| PASS_N[패스 네트워크<br>다이어그램]
        VIZ --> |성과 그래프| PERF[성과 지표<br>그래프]
        
        PERS --> S3C[S3 Content<br>가공 콘텐츠 저장]
        TEAM_H --> S3C
        GAME_H --> S3C
        HEAT --> S3C
        PASS_N --> S3C
        PERF --> S3C
    end

    %% 데이터 저장 및 API
    subgraph DB["데이터 저장 및 API"]
        direction TB
        DYNAMO[DynamoDB<br>이벤트/메타데이터] --> API
        RDS[RDS PostgreSQL<br>구조화된 통계] --> API
        S3C --> CDN[CloudFront<br>CDN]
        
        subgraph API["API 레이어"]
            APIG[API Gateway<br>REST API] --> |데이터 요청/응답| APP
            APPS[AppSync<br>실시간 GraphQL] --> |실시간 업데이트| APP
            CDN --> |미디어 콘텐츠| APP
        end
    end

    %% 최종 사용자 경험
    subgraph USER["5️⃣ 사용자 경험"]
        direction TB
        APP[모바일 앱<br>웹 대시보드] --> |개인 데이터| PHD[개인 대시보드]
        APP --> |팀 데이터| TD[팀 대시보드]
        APP --> |경기 데이터| GD[경기 대시보드]
        
        PHD --> |공유| SOCIAL[소셜 미디어<br>공유]
        PHD --> |개선점| IMPROVE[성장 분석<br>및 추천]
        TD --> LEAGUE[리그/토너먼트<br>통계]
        GD --> ARCHIVE[경기 아카이브]
    end

    %% 시스템 간 연결
    CAPTURE --> |실시간 스트리밍| KVS
    EDGE --> |로컬 처리 데이터| KVS
    CLOUD --> |처리된 영상| AI
    AI --> |분석 결과| CONTENT
    AI --> |계산된 지표| DB
    CONTENT --> |생성된 콘텐츠| DB
    DB --> |데이터 및 콘텐츠| USER

    %% 피드백 루프
    USER --> |사용자 피드백| AI
    
    %% 스타일링 (진한 배경, 흰색 텍스트, 굵은 외곽선)
    classDef camera fill:#B71C1C,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef edge fill:#424242,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef cloud fill:#0D47A1,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef ai fill:#4A148C,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef vision fill:#6A1B9A,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef action fill:#283593,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef event fill:#1565C0,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef metric fill:#0277BD,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef content fill:#2E7D32,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef storage fill:#00695C,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef api fill:#F9A825,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef app fill:#EF6C00,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef user fill:#E64A19,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    
    class V,G1,G2 camera;
    class EDGE,EP,BF,ST,LS edge;
    class CLOUD,KVS,ML,COMPUTE,EC2,ECS,BATCH cloud;
    class OD,TR,CM vision;
    class C3D,LSTM,POSE,ACTION action;
    class MULTI,SCORE,RULE,HILIGHT event;
    class MOVE,PLAYER,POS,STATS,TEAM metric;
    class CLIP,PERS,TEAM_H,GAME_H,VIZ,HEAT,PASS_N,PERF content;
    class S3R,S3C,DYNAMO,RDS storage;
    class APIG,APPS,CDN api;
    class APP,PHD,TD,GD app;
    class SOCIAL,IMPROVE,LEAGUE,ARCHIVE user;
```



## 시스템 핵심 프로세스 플로우

```mermaid
flowchart LR
    
    %% Main flow
    
    A[카메라 시스템<br>Veo + GoPro] --> B[영상 스트리밍<br>엣지 컴퓨팅]
    B --> C[AWS 클라우드<br>영상 처리]
    C --> D[AI 분석 엔진]
    
    %% AI analysis branches
    D --> E1[컴퓨터 비전<br>선수/공 추적]
    D --> E2[3D CNN + LSTM<br>행동 인식]
    D --> E3[이벤트 감지<br>멀티모달 분석]
    
    %% Outputs from AI
    E1 --> F1[지표 생성]
    E2 --> F1
    E3 --> F2[하이라이트 생성]
    
    %% Final products
    F1 --> G1[개인/팀 성과 분석]
    F2 --> G2[하이라이트 패키지]
    
    G1 --> H[모바일 앱<br>사용자 서비스]
    G2 --> H
    
    %% Feedback loop
    H --> |피드백 루프|D
    
    %% Styling (가독성 향상을 위한 진한 배경, 흰색 텍스트, 외곽선)
    classDef input fill:#D32F2F,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef process fill:#1976D2,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef aiAnalysis fill:#388E3C,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef output fill:#F57F17,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    classDef delivery fill:#4527A0,stroke:#fff,stroke-width:2px, color:#fff, font-weight:bold;
    
    class A,B input
    class C,D process
    class E1,E2,E3 aiAnalysis
    class F1,F2 output
    class G1,G2,H delivery
```

## 기술 상세 플로우

```mermaid
flowchart TD
    
    %% Input data
    Video[풋살 경기 영상<br>Veo + GoPro] --> PreProc[영상 전처리<br>프레임 추출 & 동기화]
    
    %% Computer Vision Pipeline
    PreProc --> Detection[객체 감지<br>YOLOv8]
    Detection --> Tracking[객체 추적<br>ByteTrack]
    Tracking --> Mapping[공간 매핑<br>호모그래피 변환]
    
    %% Action Recognition
    subgraph ActionRecog["행동 인식 파이프라인"]
        CNN["3D CNN (I3D)<br>시공간적 특징 추출"] --> BiLSTM["Bi-directional LSTM<br>시간적 컨텍스트 모델링"]
        BiLSTM --> ActionClass["행동 분류기<br>패스/슛/태클/드리블 등 분류"]
    end
    
    %% Event Detection
    subgraph EventDetect["이벤트 감지 시스템"]
        Multi["멀티모달 분석기<br>영상 + 오디오"] --> EventClass["이벤트 분류기<br>골/위험찬스/좋은플레이"]
        EventClass --> Scoring["중요도 점수화<br>알고리즘"]
        Scoring --> Threshold["임계값 필터링<br>(6점 이상 선정)"]
    end
    
    %% Metrics Calculation
    subgraph MetricsCalc["지표 계산 시스템"]
        MovementA["움직임 분석<br>거리/속도/가속도"] --> PlayerMetrics["개인 지표 계산"]
        ActionMetrics["기술 지표 분석<br>패스/슛/수비 성공률"] --> PlayerMetrics
        PositionA["포지셔닝 분석<br>히트맵/점유공간"] --> PlayerMetrics
        
        PlayerMetrics --> IndividualStats["개인 성과 지표"]
        PlayerMetrics --> TeamMetrics["팀 지표 집계"]
        TeamMetrics --> TeamStats["팀 성과 지표"]
    end
    
    %% Content Generation
    subgraph ContentGen["콘텐츠 생성 시스템"]
        Threshold --> ClipGen["클립 생성기<br>전후 컨텍스트 포함"]
        ClipGen --> IndHighlights["개인별 하이라이트"]
        ClipGen --> TeamHighlights["팀 하이라이트"]
        ClipGen --> FullHighlights["전체 경기 하이라이트"]
        
        IndividualStats --> DataViz["데이터 시각화"]
        TeamStats --> DataViz
        DataViz --> Dashboard["성과 대시보드"]
    end
    
    %% Pipeline Connections
    Mapping --> ActionRecog
    Mapping --> MetricsCalc
    Tracking --> EventDetect
    ActionClass --> EventClass
    ActionClass --> ActionMetrics
    
    %% Output and Delivery
    IndHighlights --> DeliverySystem["콘텐츠 전달 시스템<br>CDN & 모바일 앱"]
    TeamHighlights --> DeliverySystem
    FullHighlights --> DeliverySystem
    Dashboard --> DeliverySystem
    
    %% Styling
    classDef input fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,font-size:14px
    classDef preproc fill:#bbdefb,stroke:#1976d2,stroke-width:2px,font-size:14px
    classDef vision fill:#90caf9,stroke:#1e88e5,stroke-width:2px,font-size:14px
    classDef action fill:#c8e6c9,stroke:#43a047,stroke-width:2px,font-size:14px
    classDef event fill:#a5d6a7,stroke:#388e3c,stroke-width:2px,font-size:14px
    classDef metrics fill:#dcedc8,stroke:#689f38,stroke-width:2px,font-size:14px
    classDef content fill:#fff9c4,stroke:#fdd835,stroke-width:2px,font-size:14px
    classDef delivery fill:#ffe0b2,stroke:#f57c00,stroke-width:2px,font-size:14px

    class Video input
    class PreProc preproc
    class Detection,Tracking,Mapping vision
    class CNN,BiLSTM,ActionClass action
    class Multi,EventClass,Scoring,Threshold event
    class MovementA,ActionMetrics,PositionA,PlayerMetrics,TeamMetrics,IndividualStats,TeamStats metrics
    class ClipGen,IndHighlights,TeamHighlights,FullHighlights,DataViz,Dashboard content
    class DeliverySystem delivery
```

