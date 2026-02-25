# 스프린트 풀스택 12기 미니 프로젝트: 4팀

## 소개

- 본 프로젝트는 K-POP 아티스트 에스파(aespa)를 주제로 제작한 팬사이트입니다.

### 프로젝트 목표

- HTML 시맨틱 태그를 활용한 구조적 마크업 설계
- CSS Box Model, Display, Flexbox를 기반으로 한 레이아웃 구현
- Git Flow 전략을 적용한 브랜치 기반 협업 경험
- 역할 분담을 통한 다중 페이지 웹사이트 완성
  <br />

## 팀원 및 역할

|          [윤이준](https://github.com/yoonleejun)          |          [박소정](https://github.com/sojeong0302)          |          [유서현](https://github.com/yooseohyeon)          |          [이상윤](https://github.com/sensertive05)          |          [이지연](https://github.com/sprintjy12)          |          [최혜성](https://github.com/gptjd0204)          |          [추명곤](https://github.com/hogu-giriboy)          |
| :-------------------------------------------------------: | :--------------------------------------------------------: | :--------------------------------------------------------: | :---------------------------------------------------------: | :-------------------------------------------------------: | :------------------------------------------------------: | :---------------------------------------------------------: |
| <img src="https://github.com/yoonleejun.png" width="80"/> | <img src="https://github.com/sojeong0302.png" width="80"/> | <img src="https://github.com/yooseohyeon.png" width="80"/> | <img src="https://github.com/sensertive05.png" width="80"/> | <img src="https://github.com/sprintjy12.png" width="80"/> | <img src="https://github.com/gptjd0204.png" width="80"/> | <img src="https://github.com/hogu-giriboy.png" width="80"/> |
|                      팀장<br/>About                       |                         Community                          |                Main<br/>공통 Header/Footer                 |                          Schedule                           |                        Fan-letter                         |                         Gallery                          |                         Discography                         |

<br />

## 사용 기술

- HTML, CSS, Git/GitHub
  <br />

## 프로젝트 구조

```
...
├── index.html
├── about.html
├── discography.html
├── gallery.html
├── schedule.html
├── community.html
├── fan-letter.html
├── css/
│   ├── reset.css
│   ├── common.css
│   ├── index.css
│   ├── about.css
│   ├── discography.css
│   ├── gallery.css
│   ├── schedule.css
│   ├── community.css
│   └── fan-letter.css
├── images/
│   └── (이미지 파일들)
└── README.md
```

<br />

## 디자인 기획

- 작업을 하기 앞서 페이지의 전반적인 콘셉트와 메인 색상을 정하고, Figma를 활용해 공통 Header / Footer 컴포넌트의 ui를 설계했습니다.
  <br />

## 페이지 구성

### Main

#### 1. 레이아웃 구조

- `<header>`, `<main>`, `<footer>` 시맨틱 구조 설계
- `calc(100vh - header_height)`를 활용한 뷰포트 최적화

#### 2. Hero Section

- 메인 비주얼 이미지 및 타이틀 배치
- more 버튼 클릭 시 about 페이지로 이동

#### 3. Album Section

- Grid 레이아웃 기반 앨범 리스트 구현
- more 버튼 클릭 시 discography 페이지로 이동

#### 4. Recent Activities

- 최근 활동 콘텐츠
- Flex 기반 가로 스크롤 구현

### About

#### 1. Intro Section

- aespa 세계관(SYNK / KWANGYA) 콘셉트 소개 문구 구성
- 메인 타이틀 및 설명 텍스트 배치

#### 2. Hero Visual

- 단체 이미지 배치로 브랜드 아이덴티티 강조
- 세계관 분위기에 맞춘 비주얼 구성

#### 3. Member Section

- 멤버별 프로필 섹션 구성
- 이미지 + 텍스트 2열 레이아웃 설계

#### 4. Member Profile Detail

- 본명 / 생일 / 포지션 등 기본 정보 정리
- 카드 형태로 정보 구조화 및 가독성 개선

### Discography

#### 1. Hero Section

- 페이지 타이틀(Discography) 배치
- 상단 인트로 영역 구성

#### 2. Album Type Section

- Studio Album / Extended Play / Single / Digital Single 구분
- 앨범 유형별 섹션 분리 구조 설계

#### 3. Album Layout

- 앨범 로고, 커버 이미지, 발매일 정보 구성
- 앨범 단위 카드형 레이아웃 설계

#### 4. Tracklist Table

- 트랙 번호 / 곡명 / 비고 구조의 테이블 구성
- TITLE / 선공개 등 배지 스타일 적용

#### 5. External Link

- 각 트랙별 YouTube 링크 연결
- 새 창(target="\_blank")으로 이동 처리

### Gallery

#### 1. Hero Section

- 페이지 타이틀(GALLERY) 배치
- 실버 로고 배경 이미지로 브랜드 아이덴티티 강조

#### 2. MV Section

- aespa MV 목록 카드형 레이아웃 구성
- YouTube 썸네일 이미지 활용

#### 3. CSS Modal

- JavaScript 없이 `:target` 기반 모달 구현
- iframe을 활용한 YouTube 영상 삽입
- 닫기 버튼 클릭 시 앵커 이동 처리

#### 4. Photo Section

- aespa 사진 Grid 레이아웃 구성
- 이미지 반복 구조를 통한 갤러리 구현

#### 5. Top Button

- 페이지 하단 고정 Top 버튼 구현
- 클릭 시 상단(anchor)으로 이동 처리

### Schedule

#### 1. Hero Section

- 페이지 로고 이미지 배치
- 2025–2026 콘서트·이벤트 일정 타이틀 구성

#### 2. Concert · Tour Section

- 콘서트 및 투어 일정 테이블 구성
- 콘서트명 / 장소 / 날짜 구조 설계
- 국가별 국기 아이콘 삽입

#### 3. Award · Music Show Section

- 연말 시상식 및 음악 방송 일정 분리 구성
- 테이블 기반 일정 정리

#### 4. Brand · Event Section

- 브랜드 행사 및 기타 이벤트 일정 구성
- 일정 정보 표 형식으로 구조화

#### 5. Table Structure

- `<caption>`, `<thead>`, `<tbody>`를 활용한 시맨틱 테이블 설계
- `scope="col"` 적용으로 접근성 고려

#### 6. Top Button

- 페이지 하단 고정 Top 버튼 구현
- 클릭 시 상단(anchor)으로 이동 처리

### Community

#### 1. Write List Section

- 게시글 목록 테이블 구조 설계
- 제목 / 닉네임 / 작성일 / 조회수 / 좋아요 / 댓글 수 구성

#### 2. Write Button

- 글쓰기 아이콘 버튼 배치
- 클릭 시 write 페이지로 이동 처리

#### 3. Table Layout

- `<thead>` / `<tbody>` 구조 활용
- 게시글 요약 정보 행 단위 구성

#### 4. Pagination

- 페이지네이션 UI 구현
- 이전(<) / 다음(>) 버튼 및 페이지 번호 구성

### Fan-letter

#### 1. Hero Title

- FAN LETTER 타이틀 영역 구성
- 안내 문구(주의 메시지) 배치

#### 2. Form Layout

- 닉네임 / 이메일 / 메시지 입력 필드 구성
- `<label>`과 `<input>` 연결을 통한 접근성 고려

#### 3. Textarea

- 장문의 메시지 입력을 위한 textarea 구현
- 필수 입력(required) 속성 적용

#### 4. File Upload

- 이미지 파일 첨부 기능 구현
- `accept="image/*"` 속성으로 이미지 파일만 업로드 제한

#### 5. Submit Button

- 폼 제출 버튼 구현
- `method="post"` 구조 설계

<br />

## 공통 레이아웃 설계

피그마 시안을 기반으로 구현하되, 디자인 구현뿐만 아니라 시맨틱 마크업을 통한 접근성 확보를 목표로 설계했습니다.

### Header

- `position: sticky` 속성을 사용해 스크롤해도 헤더 상단에 고정
- 메뉴에 hover 효과 적용
- `<header>` + `<nav>` 기반 시맨틱 구조 설계
- 로고를 `<h1>`로 감싸 페이지의 최상위 제목을 명확히 정의
- 로고 이미지에 `alt="aespa"`를 제공하여 의미 전달
- `<nav>` 내부를 `<ul>`, `<li>` 구조로 작성하여 메뉴를 목록 기반 내비게이션으로 의미적으로 표현

### Footer

#### 1. 접근성 고려

SNS 아이콘은 단순 이미지가 아니라 외부 서비스로 이동하는 링크이므로, 이미지에 의미를 부여하는 대신(`alt`) 링크의 의미를 텍스트를 통해 전달하도록 설계했습니다.

```
<a href="#">
  <span class="sr-only">에스파 공식 유튜브</span>
  <img src="icon-youtube.svg" alt="" aria-hidden="true">
</a>
```

- `sr-only` 클래스로 화면에는 보이지 않지만 스크린리더에는 읽히는 텍스트 제공
- 아이콘 이미지는 정보를 전달하지 않는 시각적 표현 요소(장식 요소)이므로 `alt=""`, `aria-hidden="true"` 처리

#### 2. 정보 구조화

- 팀원과 깃허브 링크 영역을 별도로 구분하고, 팀원은 `<ul>` 기반 목록 구조로 구성
  <br />

## 협업 방식

Git Flow 전략 기반 브랜치 운영

- `main` : 최종 배포 브랜치
- `develop` : 통합 개발 브랜치
- `feature/*` : 페이지 단위 기능 브랜치 생성 후 PR 병합
- `PR` 리뷰 후 `develop` 병합 → 최종 `main` 반영
  <br />

## 프로젝트 회고

|  이름  | 회고                                                                                                                                                                                                                                                                                                                                                       |
| :----: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 윤이준 | 소개 페이지를 담당하며 협업 과정에서 Git 동기화의 중요성을 크게 느꼈다. 원격 저장소 변경 사항을 제때 pull하지 않아 충돌이 반복되었고, 결국 새 브랜치를 만들어 git push --force로 병합을 마무리했다. 이번 경험을 통해 구현 능력뿐만 아니라 팀원들과의 코드 싱크를 꾸준히 맞추는 습관이 협업에서 얼마나 중요한지 깨닫게 되었다.                              |
| 박소정 | AI의 도움을 최소화하며 진행해 시간이 더 걸렸지만, 그만큼 더 깊이 배우고 Git에도 익숙해지는 의미 있는 경험이었다. 인상 깊었던 점은, 문제가 생기면 모두가 마치 자신의 일처럼 화면을 공유하며 함께 해결해주려고 했다는 것이다. 그 모습에서 팀원들이 좋은 분들이라는 게 느껴졌다.                                                                              |
| 유서현 | 이번 미니 프로젝트를 진행하며 협업의 중요성을 다시 한 번 느낄 수 있었습니다. 각자의 역할을 맡아 작업했지만, 공통 레이아웃과 컨벤션을 맞추는 과정에서 팀원들과의 소통이 무엇보다 중요하다는 것을 체감했습니다. 특히 PR과 코드 리뷰를 통해 단순히 기능 구현을 넘어서 더 나은 구조와 가독성을 고민해볼 수 있었던 점이 의미 있었습니다.                        |
| 이상윤 | 스케줄 페이지를 개발하며 여러 시행착오를 겪었고, 특히 Git 작업 초기 설정 문제로 수정 과정에서 어려움을 겪었다. 발표 직전까지 수정이 이어졌지만 팀원들의 도움으로 마무리할 수 있었고, 이번 경험을 통해 기초를 더 탄탄히 다져 다음 프로젝트에서는 더 성장한 모습을 보이고자 다짐하게 되었다.                                                                 |
| 이지연 | 이번 프로젝트에서는 개발에 앞서 기획과 콘셉트 통일의 중요성을 먼저 고민했고, Figma를 활용해 방향성을 정한 뒤 작업을 시작한 점이 특히 인상 깊었다. 또한 Git 충돌이나 문제 상황에서도 팀원들이 서로의 일처럼 함께 해결하며 협업의 의미를 느낄 수 있었고, 결국 기술보다 더 중요한 것은 소통이라는 것을 다시 한 번 깨닫는 시간이었다. 누가 뭐래도 우리팀 최고! |
| 최혜성 | 이번 미니 프로젝트를 진행하며 저번 초미니 프로젝트보다 팀원들간의 소통이 훨씬 많아졌다는 것을 느꼈고 프로젝트를 진행하며 발생했던 여러 문제들을 함께 해결해나가며 제가 몰랐던 부분도 배우게 되면서 한걸음 더 성장한 것 같습니다.                                                                                                                           |
| 추명곤 | GitHub를 통한 협업 과정을 직접 경험해볼 수 있었던 프로젝트였습니다. 그리고 오류가 발생할 때마다 함께 원인을 고민하고 해결하는 과정이 특히 인상 깊었습니다. 기술적인 성장뿐 아니라 소통의 중요성을 다시 한 번 느낄 수 있는 경험이었습니다.                                                                                                                  |

<br />

## 실행 방법

```
git clone https://github.com/yoonleejun/aespa_miniproject.git
```

프로젝트를 clone한 뒤, 루트 디렉토리의 `index.html` 파일을 브라우저에서 실행합니다.
