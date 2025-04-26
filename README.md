# 📚 Think-Deeper 로컬 실행 가이드

## 🛠 프로젝트 구조
```
Think-Deeper/
├── backend/    # FastAPI 백어드
└── frontend/   # Next.js 프론티어드
```

---

## 🚀 백엔드 실행 (FastAPI)

### 1. backend 폴더로 이동
```bash
cd Think-Deeper/backend
```

### 2. 가상환경 생성 및 활성화
```bash
# 가상환경 생성
python -m venv venv

# 가상환경 활성화 (Windows)
venv\Scripts\activate
```

### 3. 패키지 설치
```bash
pip install -r requirements.txt
```
> ⚠️ Windows에서는 `uvloop` 설치 오류가 발생할 수 있으나 무시해도 됩니다.

### 4. .env 파일 복사 (필요 시)
```bash
rename .env.exapmple .env
```

### 5. 서버 실행
```bash
uvicorn app.main:app --reload
```

- FastAPI 서버: [http://localhost:8000](http://localhost:8000)
- API 문서(Swagger UI): [http://localhost:8000/docs](http://localhost:8000/docs)

---

## 🌟 프론트엔드 실행 (Next.js)

### 1. frontend 폴더로 이동
```bash
cd ../frontend
```

### 2. 패키지 설치
```bash
npm install
```

### 3. 개발 서버 실행
```bash
npm run dev
```

- 웹사이트 접속: [http://localhost:3000](http://localhost:3000)

---

## 📋 실행 요약

| 항목            | 명령어                              | 주소 |
|-----------------|--------------------------------------|------|
| 백엔드 실행     | `uvicorn app.main:app --reload`      | [http://localhost:8000](http://localhost:8000) |
| API 문서 확인   | -                                    | [http://localhost:8000/docs](http://localhost:8000/docs) |
| 프론트엔드 실행 | `npm run dev`                        | [http://localhost:3000](http://localhost:3000) |

---

## 🔥 Git 기본 사용법

### 📥 1. 원격 저장소에서 최신 내용 받아오기 (pull)

```bash
git pull origin main
```
> 다른 브랜치를 쓰면 `main`대신 브랜치명을 입력하세요.

---

### 🛠️ 2. 파일 변경사항 스테이지에 추가 (add)

```bash
git add .
```

---

### 📝 3. 커미팅 만들기 (commit)

```bash
git commit -m "변경 내용 요약 메시지"
```

---

### 🚀 4. 원격 저장소로 업로드 (push)

```bash
git push origin main
```

---

## 📢 Git 주의사항
- 협조 사고를 막기 위해 하지만 **프리 푸르(pull) 후에** 작업하세요.
- 커미팅는 간편하고 명확한 메시지로 작성해주세요.
- 충분(콤터플)이 발생하면 add → commit → push 해주세요.

---

## ✨ 기술 스택
- **백어드**: FastAPI, Python
- **프론티어드**: Next.js, React, TypeScript, TailwindCSS

---

# 👌 Happy Hacking!
