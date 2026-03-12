# 타임박스 플래너 PWA — 앱 설치 가이드

## 📱 방법 1: 깃허브 페이지 (추천, 무료)

### 1단계: GitHub 계정 생성/로그인
https://github.com 에서 로그인

### 2단계: 새 저장소 생성
1. 우상단 **+** → **New repository**
2. Repository name: `timebox` (아무 이름)
3. **Public** 선택
4. **Create repository** 클릭

### 3단계: 파일 업로드
1. **uploading an existing file** 클릭
2. 이 폴더의 모든 파일(index.html, manifest.json, sw.js, icons/)을 드래그 업로드
3. **Commit changes** 클릭

### 4단계: GitHub Pages 활성화
1. 저장소 → **Settings** → 좌측 **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** / **(root)** → **Save**
4. 1~2분 후 `https://사용자명.github.io/timebox/` 접속 가능

### 5단계: 앱 설치
1. 폰 Chrome에서 위 URL 접속
2. 주소창 옆 **설치** 아이콘 클릭 (또는 메뉴 → "앱 설치")
3. 홈 화면에 앱 아이콘 생성됨!

---

## 💻 방법 2: PC에서 로컬 테스트

```bash
# 이 폴더에서:
python3 -m http.server 8080

# 또는
npx serve .
```
브라우저에서 `http://localhost:8080` 접속

---

## 📁 파일 구조
```
PWA/
├── index.html       ← 타임박스 플래너 앱
├── manifest.json    ← PWA 설치 설정
├── sw.js            ← 오프라인 캐시
├── icons/
│   ├── icon-192.png ← 앱 아이콘 (192px)
│   └── icon-512.png ← 앱 아이콘 (512px)
└── README.md
```
