# 2025-spring-ewha-capston-design
This is Team35:Tricode's 2025-spring-ewha-capston-design repository.

# Team-Info
| (1) 과제명 | 학원강사와 수강생의 분산된 학습 자료 통합 관리 및 정확한 정보 탐색을 위한 RAG 기반 개인 맞춤 챗봇 서비스
|:---  |---  |
| (2) 팀 번호 / 팀 이름 | *35-트리코드* |
| (3) 팀 구성원 | 황혜진 (2217040): 리더, 백엔드 및 AI 개발 담당, 챗봇 API 구현 및 Flask API와의 연결 진행, 유사도 검색 Flask API 구현<br> 장예주 (2276267): 팀원, 프론트엔드 개발 담당, 주요 페이지 디자인 설계 및 백엔드와 API 연동 진행, 통합테스트 진행<br> 오민지 (2217021) : 팀원, 백엔드 및 AI 개발 담당, 회원가입 및 인증 API와 파일 업로드 및 저장 API 개발, 문서 로드 기능 구현 및 청크 분할 코드 |
| (4) 팀 지도교수 | 용환승 교수님 |
| (5) 과제 분류 | *산학과제* |
| (6) 과제 키워드 | *RAG, chatGPT, 학습 질의응답*  |
| (7) 과제 내용 요약 | 학습 자료에서 모르는 부분에 대해 정확한 설명을 얻기 힘들고, 파일이 분산 저장되어 있어 필요한 내용이 어디있는지 찾기 힘든 수강생과 학습자료를 효율적으로 관리하고, 많은 학습 자료로 학습 준비에 어려움을 겪는 학원강사를 위하여 RAG구조를 이용한 학습자료 통합 저장 기능과 학습 자료를 기반으로 정확한 응답 생성 및 자료 위치 탐색 기능을 제공하여 학습을 돕는 챗봇 서비스 |

<br>

# Project-Summary
## (1) 문제 정의
 학원강사는 반복적인 질의응답으로 업무 부담이 크고, 질문 조교를 고용해도 답변의 일관성과 정확성이 떨어지며 인건비 부담이 있다. 수강생은 학습 자료가 분산 저장되어 필요한 내용을 찾기 어렵고, 즉각적인 질문 해결이 불가능해 학습 효율이 저하된다.<br>이를 해결하기 위해 RAG 기반 챗봇 서비스를 도입하여 학습 자료를 통합 저장하고, AI를 활용해 정확한 답변을 제공함으로써 강사의 업무 부담을 줄이고, 수강생들이 언제 어디서나 필요한 정보를 쉽게 찾고 궁금증을 해결할 수 있도록 한다.
<br>

## (2) 기존연구와의 비교 
**1. chatGPT와 Edu've비교**
<br>
<img width="365" alt="Image" src="https://github.com/user-attachments/assets/a6971ad3-c924-4a11-96dd-9d6c87a2ff6c" />
<br>
**2. Notion과 Edu've비교**
<br>
<img width="368" alt="Image" src="https://github.com/user-attachments/assets/4fae52f6-697a-4ef0-9768-c2c3d003375b" />
<br>
   Edu've는 학습자료 기반의 정확한 답변 제공, 강력한 문서 검색 기능, 맞춤형 학습 지원, 실시간 학습 피드백, 효율적인 학습자료 관리를 통해 ChatGPT와 Notion보다 수강자와 강사에게 최적화된 솔루션을 제공한다.<br>
   RAG 구조를 활용하여 학습자료와 연계된 신뢰도 높은 답변을 제공하고, 벡터 검색으로 문서 내 특정 내용을 정확하게 탐색할 수 있다. 또한, AI 챗봇을 통해 24시간 실시간 피드백을 제공하고, 개인 맞춤형 학습 경험을 지원하여 학습 공백을 최소화한다.

## (3) 제안 내용 
**1. 학습 자료 통합 저장 및 관리**
<br>학원에서 제공하는 학습자료를 RAG 구조를 활용하여 아카이브에 저장함으로써, 수강생과 학원강사가 쉽게 필요한 자료를 찾고 활용할 수 있도록 한다. 이때, 학습자료는 PDF, 워드 파일, 이미지, 음성 강의 등 다양한 형식의 자료를 디지털화하여 관리한다. 또한, 학원강사는 자료를 실시간으로 업데이트할 수 있으며, 수강생들은 최신 학습자료를 즉각적으로 확인할 수 있어 효율적인 학습 환경을 조성할 수 있다.<br> 
**2. AI 기반 맞춤형 질의응답 시스템**
<br> ChatGPT를 기반으로 하되, 학원의 학습자료를 반영하여 수강생의 질문에 답변함으로써 기존의 학습자료와의 연계성을 유지하며 더욱 정확하고 신뢰할 수 있는 답변을 제공한다. 또한, 설명 난이도와 말투 조절 기능을 적용해 수강생의 이해 수준과 선호도에 따라 답변을 조정하여 수강생 개개인의 이해도를 높일 수 있도록 맞춤형 학습을 지원한다. 

## (4) 기대효과 및 의의
**1. 학습자료의 체계적 관리 및 시공간 제약 극복으로 학습 효율성 증대**
<br> Edu've는 학원의 모든 학습자료를 RAG구조로 통합 저장하고 체계적으로 관리할 수 있도록 하여, 수강생과 강사가 언제든지 필요한 자료에 접근할 수 있으며, 중복 자료 문제를 줄이고 활용도를 극대화할 수 있다. 또한, Edu've는 AI 기반 질의응답 시스템을 통해 수강생들이 언제 어디서나 학습자료를 탐색하고 질문할 수 있도록 지원하여 학습 효율성을 극대화한다. 24시간 운영 가능한 AI 챗봇은 실시간으로 정확한 답변을 제공하여 학습 공백을 최소화하고, 지속적인 학습이 가능하도록 돕는다. 
<br> **2. 강사의 업무 부담 감소 및 강의 품질 향상**
<br> 강사는 반복적인 질의응답에서 벗어나 강의 준비와 개별 수강생의 학습 지도에 더욱 집중할 수 있다. 기존에는 질문 조교를 고용해 수강생들의 질문을 처리했지만, 답변의 일관성과 정확성을 유지하기 어려웠으며 인건비 부담도 컸다. Edu've는 강사의 강의 내용을 반영한 정확한 답변을 제공하여 강사의 업무를 보완하고, 보다 체계적인 학습 환경을 조성할 수 있도록 한다.
<br> **3. 개인 맞춤형 학습 지원**<br> 
Edu've는 수강생 개개인의 학습 스타일과 이해 수준을 고려하여 맞춤형 학습을 지원한다. 설명 난이도 및 말투를 조절해 사용자의 수준에 맞는 답변을 제공하여 사용자에게 더욱 효과적인 학습 경험을 제공할 수 있다.
<br> **4. 지속적인 AI 성능 향상 및 데이터 활용 가치 극대화**<br> 
Edu've는 학습자료와 사용자의 상호작용 데이터를 지속적으로 축적하며, 이를 통해 서비스 성능을 점차 개선한다. 시간이 지날수록 축적된 학습자료와 질문 패턴을 기반으로 Edu've는 점점 더 정확하고 정교한 답변을 제공할 수 있게 된다. 또한, 수강생들의 학습 경향을 분석하여 각 사용자에게 맞춤형 답변을 제공하는 등 학습을 최적화하고 사용자의 성장을 지원하는 서비스를 제공한다. 
## (5) 주요 기능 리스트 
**1. 학습 자료 업로드 및 보관** ; 강사와 수강생이 강의 자료 및 필기 내용을 한 곳에서 보관, 업로드 및 관리할 수 있도록 지원
 - 다양한 형식 지원: PDF, 이미지, 텍스트 파일 등 여러 형식의 학습 자료를 업로드할 수 있다.
 - 자동 텍스트 추출: 업로드된 문서 및 이미지 내 텍스트를 자동으로 추출하여 검색이 용이하도록 저장한다.
 - 폴더별 정리 및 탐색: 사용자가 폴더를 생성하여 자료를 체계적으로 정리하고, 빠르게 검색 가능
 - 실시간 업데이트: 새 자료 추가 및 기존 자료 수정 시 즉시 반영하여 최신 상태 유지

**2. 음성 강의 자동 텍스트 변환** ; 강의 녹음 파일을 업로드하면 AI가 자동으로 텍스트로 변환하여 학습 자료로 활용할 수 있도록 지원

- AI 기반 음성 인식: 업로드된 음성을 자동으로 텍스트로 변환하여 학습 자료로 저장한다.
- 효율적인 학습 지원: 변환된 텍스트는 검색이 가능하도록 처리되어, 필요한 내용을 빠르게 확인할 수 있다.
- 강의 복습 용이: 음성 파일을 다시 들을 필요 없이, 텍스트로 변환된 내용을 통해 강의를 효과적으로 복습할 수 있다.

**3. AI 챗봇을 통한 실시간 질문 응답** ; RAG 구조를 활용하여 학습 자료 기반의 정확한 질의응답을 제공

- 학습 자료 기반 응답: 일반적인 AI 챗봇과 달리, 학원에서 제공한 학습 자료를 기반으로 답변을 생성한다.
- 유사도 검색 기능: 사용자가 질문을 입력하면, AI가 관련 학습 자료를 검색하여 정확한 답변을 제공한다.
- 학습 자료 위치 안내: 질문에 대한 답변과 함께, 해당 내용을 포함한 학습 자료의 위치를 제공하여 빠르게 필요한 정보를 찾을 수 있도록 지원한다.

**4. 맞춤형 챗봇 설정** ; 사용자의 학습 스타일과 선호도에 맞춰 챗봇을 개인화할 수 있도록 다양한 설정 기능을 제공

- 챗봇 개인화 설정: 사용자는 챗봇의 이름을 설정하고, 말투(친근한/정중한 등)와 설명 난이도를 조절할 수 있다.
- 프롬프트 엔지니어링을 이용한 개인 맞춤화: AI는 사용자의 질문 패턴을 분석하여 더욱 정교하고 맞춤형 답변을 제공한다.

<br>
 
# Project-Design & Implementation

## (1) 요구사항 정의  
### 기능별 상세 요구사항

**1. 학습 자료 업로드 기능**
 - 사용자(선생님, 학생)는 학습자료(강의 자료/노트 필기)를 업로드하여 한 곳에 보관 할 수 있다.
 - 학생 사용자는 선생님이 업로드한 강의 자료를 조회할 수 있다.

✅ **기능 상세 설명**
 - 사용자가 파일(PDF, 이미지, 텍스트 등)을 업로드하면 서버에서 저장
 - Langchain 라이브러리를 사용하여 문서 및 이미지 내 텍스트를 추출
 - 업로드된 자료를 벡터 DB에 임베딩하여 검색 가능하게 처리

✅ **입력 및 출력**
- 입력: 파일(PDF, 이미지, TXT 등)
- 출력: 서버에 파일 저장 → 결과데이터 출력(파일 ID)

<br> 

**2. STT(Speech-to-Text) 기능**
- 사용자는 음성파일을 업로드하면 텍스트로 변환된 문서를 볼 수 있다.

✅ **기능 상세 설명**
- 사용자가 음성 파일을 업로드하면 daglo STT API를 호출하여 텍스트 변환
- 변환된 텍스트를 벡터 DB에 임베딩
- 결과를 사용자에게 반환 / 사용자가 조회 할 수 있도록 학습자료DB에 저장

✅ **입력 및 출력**
- 입력: 음성 파일
- 출력: 텍스트 파일 저장 및 출력

<br> 

**3. RAG 기반 챗봇 기능**
- 사용자의 질문을 이해하고, 학습 자료를 기반으로 최적의 답변 제공한다.

✅ **기능 상세 설명**
- 사용자가 질문을 입력하면 벡터 DB에서 유사도 검색을 통해 문서를 검색 후 ChatGPT API를 호출하여 응답 생성
- 검색된 문서를 바탕으로 답변을 생성하여 챗봇 응답의 정확도를 높임
- 사용자가 챗봇에게 학습 자료의 위치 및 학습 내용에 대해 질문할 수 있음

✅ **입력 및 출력**
- 입력: 사용자의 질문(학습 자료 관련 내용/위치 질문 포함)
- 출력: ChatGPT 기반의 답변(학습 자료 위치 및 내용 안내)

<br> 

**4. 챗봇 개인 설정 기능**
- 사용자는 챗봇의 이름,말투, 설명 난이도 등을 자신의 선호에 맞게 설정할 수 있다.

✅ **기능 상세 설명**
- 사용자가 챗봇의 이름을 설정할 수 있음
- 챗봇의 말투(정중한/친근한 등)와 답변 난이도를 조정할 수 있음
- 설정한 값은 사용자별로 저장되며, 이후 채팅 시 반영됨

✅ **입력 및 출력**
- 입력: 챗봇 설정 값(이름, 말투, 설명 난이도 등)
- 출력: 설정 값 저장 및 결과 출력

<br> 

**5. 학습 자료 폴더 정리 기능**
- 사용자는 폴더를 생성하여 업로드한 학습 자료를 자신이 원하는 대로 정리할 수 있다.

✅ **기능 상세 설명**
- 사용자가 폴더를 생성하고 원하는 학습 자료를 추가 및 이동 가능
- 폴더별로 자료를 정리하여 손쉽게 탐색할 수 있도록 지원

✅ **입력 및 출력**
- 입력: 폴더 생성 요청(폴더명, 설명, 포함할 자료 리스트)
- 출력: 생성된 폴더 ID 및 학습 자료 목록 출력



## (2) 전체 시스템 구성 

![image](https://github.com/user-attachments/assets/458274e5-e5b3-4a8c-be2a-63d9f5fb1b30)

- **리액트 UI:** 사용자 입력(사용자 정보, 질문, 학습 자료 업로드) 제공.

- **사용자 관리 모듈:** 사용자 인증 및 권한 관리 (학생/선생님 역할 부여).
  
- **학습 자료 관리 모듈:** 사용자가 업로드 한 자료를 S3, MySQL에 저장하고 필요 시 STT(daglo STT API) 변환 수행.
  
- **RAG 시스템:** Flask에서 OpenAI embeddign과 LangChain 사용하여 학습 자료를 임베딩 후 벡터 DB(ChromaDB)에 저장하고 유사도 검색 수행.
  
- **질의응답 모듈:** 질문을 분석하고 RAG 시스템에서 관련 학습 자료 검색.
  
- **ChatGPT:** 검색된 자료를 바탕으로 답변 생성.
  
- **맞춤형 챗봇 설정 모듈:** 사용자의 선호 설정(말투, 설명 난이도, 응답 선호도 분석 기록)을 반영하여 최종 응답 제공.


## (3) 주요엔진 및 기능 설계
**1. 사용자 관리 모듈**

- **역할:** 사용자 인증 및 권한 관리 (학생/선생님 역할 부여)
- **사용 기술:** Spring Security, JWT
- **주요 서비스 구현:**
    - **회원가입 및 로그인 기능:**
        - 사용자의 이메일 및 비밀번호를 기반으로 가입 및 로그인
        - 비밀번호 해싱 (BCrypt 암호화 사용)
    - **JWT 토큰 기반 인증 및 인가:**
        - 로그인 성공 시 JWT 토큰 발급
        - Spring Security의 OncePerRequestFilter를 활용한 토큰 검증
        - 사용자 역할(Role-Based Access Control) 적용 (학생 / 선생님 구분)
    - **사용자 정보 관리:**
        - 사용자 정보 MySQL에 저장
        - 프로필 정보 조회 및 수정 기능 제공

 **2. 학습 자료 업로드 모듈** 

- **역할:** 사용자가 업로드한 학습 자료 저장 및 관리
- **사용 기술:** Spring Boot, MySQL, S3, daglo STT (음성 → 텍스트 변환)
- **주요 서비스 구현:**
    - **파일 업로드 (`FileUploadService`)**
        - MultipartFile을 이용한 파일 업로드 기능
        - 업로드된 파일을 Amazon S3에 저장하고, 해당 파일의 메타데이터를 MySQL에 저장
    - **음성 자료 변환 (daglo STT API 연동)**
        - 사용자가 음성 자료 업로드 시, STT (Speech-to-Text) 변환 수행
        - 변환된 텍스트 파일을 학습 자료로 활용할 수 있도록 저장
    - **파일 메타데이터 관리 (`MySQL`, `ChromaDB`)**
        - 저장된 학습 자료의 파일명, 업로드 시간, 타입 등을 관리

 **3. 질의응답 모듈** 
- **역할:** 사용자의 질문을 받아 적절한 답변을 생성하는 기능 수행
- **사용 기술:** Flask, LangChain, ChatGPT API
- **주요 서비스 구현:**
    - **질문 전처리 (`ChatService`)**
        - 사용자의 질문을 자연어 처리(NLP)하여 이해
        - 불필요한 문구 제거 및 정제된 질문 생성
        - 질문을 적절한 형식으로 변환하여 RAG 시스템과 통신
        - 답변을 사용자에게 전달
    - **대화 기록 관리 (`ConversationService`)**
        - 사용자의 대화 히스토리 저장 (맥락 유지)
    - **메시지 서비스 (`MessageService`)**
        - 특정 사용자의 대화 기록을 조회하는 기능 제공

 **4. RAG 시스템** 

- **역할:** 학습 자료를 벡터화하여 유사도 검색을 수행하고, 검색된 정보를 바탕으로 챗봇 응답 생성
- **사용 기술:** OpenAI embedding, ChromaDB, LangChain
- **주요 서비스 구현:**
    - **임베딩 변환 (`Embedding Module`)**
        - 학습 자료를 OpenAI embedding을 사용하여 벡터 변환
        - 변환된 벡터를 벡터 데이터베이스(ChromaDB)에 저장
    - **유사도 검색 (`Similarity Search Module`)**
        - 사용자의 질문을 벡터로 변환 후, ChromaDB에서 가장 유사한 문서를 검색
        - 검색된 문서를 기반으로 ChatGPT에 전달하여 응답 생성

 **5. 맞춤형 챗봇 설정 모듈** 

- **역할:** 사용자의 학습 스타일과 선호도에 맞춰 챗봇을 개인화
- **사용 기술:** Flask, LangChain, MySQL
- **주요 서비스 구현:**
    - **사용자 설정 관리 (`UserCharacterService`)**
        - 사용자가 챗봇의 말투(친근한/정중한), 설명 난이도 등을 설정 가능
        - 사용자별 설정 정보를 MySQL에 저장
    - **개인화된 프롬프트 엔지니어링**
        - 사용자의 질문 패턴을 분석하여 맞춤형 답변 제공
        - 질문을 변환하여 챗봇이 더 정교하게 응답할 수 있도록 보정
    - **응답 후처리**
        - ChatGPT의 응답을 사용자의 스타일에 맞게 변환

 **6. 데이터 저장 및 관리** 

- **MySQL:** 사용자 정보, 학습 자료 메타데이터, 챗봇 설정 정보 저장
- **ChromaDB:** 학습 자료의 임베딩 벡터 저장 및 유사도 검색
- **S3:** 업로드된 학습 자료(파일) 저장

## (4) 주요 기능의 구현 
### 1. RAG 기반 챗봇 기능
사용자가 질문을 입력하면 벡터 DB에서 유사한 문서를 검색하고, 이를 바탕으로 ChatGPT API를 호출하여 학습 자료에 기반한 정확한 답변을 하도록 함
- **POST /chat/start**
- **Input**: 사용자의 질문 텍스트
- **Output**: 사용자가 질문한 내용의 대한 답변 텍스트

(1) 유사도 검색 flaskAPI
```python
@app.route('/search', methods=['POST'])
def search():
    try:
        data = request.json
        query = data.get("query", "")
        
        if not query:
            return jsonify({"error": "No query provided"}), 400
```
`request.json`을 사용하여 클라이언트가 보낸 JSON 데이터(사용자의 질문)를 가져와서 질문 내용만 추출한다.

<br>

```python
retriever = vectorstore.as_retriever()
docs = retriever.invoke(query)
```
벡터 데이터베이스에서 유사도 검색할 수 있는 retriever 객체를 생성한다.
<br>`retriever.invoke(query)` 로 사용자 질문을 기반으로 유사한 문서를 검색한다.

<br>

```python
results = [{"page": doc.metadata["page"], "content": doc.page_content} for doc in docs]
return jsonify({"results": results})
```
검색된 문서에서 페이지 번호와 문서 내용으로 구성된 JSON으로 변환하여 응답을 반환한다.

<br>

(2) 유사도 검색 결과를 이용하는 챗봇
```java
public MessageUnitDto startConversation(MessageRequestDto requestDto, Long userId) throws JsonProcessingException{
        
        String userMessage = requestDto.getQuestion();
        // 사용자 메시지 저장
        Message message = conversationService.processUserMessage(userId, userMessage);
        // 유사도 검색 flaskAPI 호출
        String similarDocuments = flaskComponent.findSimilarDocuments(userMessage);
```
사용자의 질문을 받아 해당 메시지를 데이터베이스에 저장한다.
`flaskComponent.findSimilarDocuments(userMessage);`에서 유사도검색 flask API를 호출하여 유사도 검색을 수행한다.

<br>

```java
       // ChatGPT API 호출
        ResponseEntity<String> response= chatGptClient.chat(userMessage, similarDocuments);
        String parsedResponse = parseResponse(response);

        // 챗봇 응답 저장
        Message botMessage = Message.createBotResponse(message.getConversation(), parsedResponse, message);
        conversationService.saveBotMessage(botMessage);

        return MessageUnitDto.from(message,botMessage);
    }
```
`chatGptClient.chat()` 메서드는 사용자의 질문과 유사 문서(문서내용,페이지 번호)를 함께 ChatGPT API로 전달하여 그에 맞는 응답을 받고 이를 반환한다.

<br>

### 2. 학습자료 임베딩 기능 구현
사용자가 업로드한 학습 자료(PDF, 텍스트 등)를 임베딩 모델을 사용하여 벡터화 후 저장하여 이후 유사도 검색이 가능하게 함
- **POST /embedding**
- **Input**: pdf, docx, 이미지(jpg, jpeg, png), 텍스트(txt) 등 다양한 형식의 학습자료 파일
- **Output**: X

<br>

(1) 파일 형식별 변환 처리
```python
@app.route('/embedding', methods=['POST'])
def embed_pdf():
    processed_path = None
    # 파일 종류별 텍스트로 변환 로직
    if file_ext == 'pdf': # pdf 파일이면 그대로 진행
        processed_path = filepath
    elif file_ext == 'docx': # docx
        processed_path = filepath.replace('.docx', '.pdf')
        convert_docx_to_pdf(filepath, processed_path)
    elif file_ext in ['jpg', 'jpeg', 'png']: # 이미지
        text = extract_text_from_image(filepath)
    elif file_ext == 'txt': # txt
        with open(filepath, 'r', encoding='utf-8') as file:
            text = file.read() 
```
dox 파일 : `convert_docx_to_pdf(filepath, processed_path)`로  **PDF로 변환한다.**
<br>이미지 : `extract_text_from_image(filepath)`로 업로된 이미지에서 텍스트를 추출한다.
<br>텍스트 파일 : `text = file.read()`를 통해 파일을 열어 **내용을 읽는다.**

<br>

(2) pdf 처리 및 텍스트 전처리
```java
docs = []
if processed_path:
    loader = PyMuPDFLoader(processed_path)
    docs = loader.load()
```
`PyMuPDFLoader`와 **`loader.load()`**를 사용하여 PDF 파일을 로드하고 내용을 텍스트로 추출한다.

<br>

(3) 청크 분할 및 메타데이터 생성
```python
    text_splitter = RecursiveCharacterTextSplitter(chunk_size=500, chunk_overlap=50)
    split_documents = []

    for doc in docs:
        page_content = doc.page_content
        page_number = doc.metadata['page'] 
        # 페이지 내용을 청크 단위로 분할
        split_page_content = text_splitter.split_text(page_content)
        # 각 청크에 페이지 번호를 추가하고 메타데이터 생성
        for chunk in split_page_content:
            split_documents.append({
                "content": chunk.strip(),
                "metadata": {"page": page_number}
            })
       
      contents = [doc["content"] for doc in split_documents]
      metadatas = [doc["metadata"] for doc in split_documents]
```
`text_splitter`: `RecursiveCharacterTextSplitter`를 이용하여 텍스트를 청크로 분할한다.
<br>`chunk_size=500`은 한 청크의 최대 크기가 500자로 설정되며,  `chunk_overlap=50`은 각 청크가 겹치는 부분을 50자로 설정하여 문맥을 유지할 수 있도록 한다.
<br>분할한 청크의 문서 내용은 “content”, 페이지번호는 “metadata”로 분할한다.

<br>

(4) 텍스트와 메타데이터를 벡터데이터베이스에 추가
```python
vectorstore.add_texts(texts=contents, metadatas=metadatas)
vectorstore.persist()
```
`vectorstore.add_texts(texts=contents, metadatas=metadatas)`를 이용하여 벡터데이터베이스에 데이터를 저장한다. 

