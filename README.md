# 🔍 심층 웹 리서치 자동 보고서 생성기

웹 데이터를 탐색하거나 업로드한 문서를 분석하여 기사형 보고서를 자동으로 생성하는 도구입니다.

## 주요 기능

- **웹 데이터 수집**: Firecrawl API를 활용한 웹 데이터 자동 수집
- **문서 분석**: PDF 및 Word 문서 업로드를 통한 텍스트 및 이미지 추출
- **보고서 생성**: 수집된 정보를 토대로 기사형 보고서 자동 생성
- **다양한 출력 형식**: DOCX, PDF 형식으로 다운로드 지원

## 설치 방법

1. 저장소 클론
   ```
   git clone https://github.com/quentinjeon/pdf_news.git
   cd pdf_news
   ```

2. 필요 패키지 설치
   ```
   pip install -r requirements.txt
   ```

3. 환경 설정
   - `.env.example` 파일을 `.env`로 복사하고 API 키 입력
   ```
   cp .env.example .env
   ```
   - `.env` 파일에 OpenAI API 키와 Firecrawl API 키 입력

## 실행 방법

```
streamlit run app.py
```

## 필요 API 키

- **OpenAI API 키**: GPT 기반 보고서 생성에 사용
- **Firecrawl API 키**: 웹 데이터 수집에 사용

## 사용 방법

1. 질문 또는 주제 입력
2. 참조할 도메인 지정 (선택사항)
3. 문서 업로드 (선택사항)
4. 보고서 생성 옵션 설정 (사이드바)
5. '보고서 생성하기' 버튼 클릭
6. 결과 보고서 탭에서 생성된 보고서 확인 및 다운로드

## 기술 스택

- **Streamlit**: UI 구현
- **Firecrawl API**: 웹 데이터 수집
- **OpenAI API**: 텍스트 생성
- **PyMuPDF, python-docx**: 문서 분석
- **Python**: 백엔드 처리
