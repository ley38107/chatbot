# HyperCLOVA X SEED 테스트 프로젝트

이 프로젝트는 네이버 클라우드 플랫폼의 HyperCLOVA X SEED 모델을 테스트하기 위한 프로젝트입니다.

## 🚀 시작하기

### 1. 가상환경 설정
```bash
# 가상환경 생성
python -m venv venv

# 가상환경 활성화 (Windows)
venv\Scripts\activate

# 가상환경 활성화 (macOS/Linux)
source venv/bin/activate
```

### 2. 의존성 설치
```bash
pip install -r requirements.txt
```

### 3. 환경 변수 설정
```bash
# env_example.txt를 .env로 복사
copy env_example.txt .env

# .env 파일 편집하여 API 키 설정
```

### 4. API 키 발급
1. [네이버 클라우드 플랫폼](https://www.ncloud.com/) 계정 생성
2. HyperCLOVA X SEED 서비스 신청
3. API 키 발급 및 .env 파일에 설정

## 📁 프로젝트 구조
```
LLM/
├── requirements.txt          # Python 의존성
├── env_example.txt          # 환경 변수 예시
├── .env                     # 실제 환경 변수 (생성 필요)
├── config.py                # 설정 관리
├── hyperclova_client.py     # HyperCLOVA API 클라이언트
├── test_hyperclova.py       # 기본 테스트 스크립트
├── streamlit_app.py         # 웹 대시보드
└── README.md                # 프로젝트 문서
```

## 🧪 테스트 실행

### 기본 테스트
```bash
python test_hyperclova.py
```

### 웹 대시보드 실행
```bash
streamlit run streamlit_app.py
```

## 📋 주요 기능

- ✅ API 연결 테스트
- 💬 텍스트 생성 테스트
- 📚 교육용 콘텐츠 테스트
- 🎛️ 파라미터 조정 (temperature, top_p, max_tokens)
- 📝 프롬프트 히스토리 관리
- 🌐 웹 기반 테스트 인터페이스

## ⚠️ 주의사항

1. **API 키 보안**: .env 파일을 .gitignore에 추가하여 API 키가 노출되지 않도록 주의하세요.
2. **API 사용량**: API 호출 시 비용이 발생할 수 있으니 사용량을 모니터링하세요.
3. **네트워크**: 안정적인 인터넷 연결이 필요합니다.

## 🔧 문제 해결

### API 연결 실패
- API 키가 올바르게 설정되었는지 확인
- 네이버 클라우드 플랫폼 계정 상태 확인
- 네트워크 연결 상태 확인

### 모듈 import 오류
- 가상환경이 활성화되었는지 확인
- requirements.txt의 패키지들이 설치되었는지 확인

## 📞 지원

문제가 발생하면 네이버 클라우드 플랫폼 고객 지원센터에 문의하세요.
