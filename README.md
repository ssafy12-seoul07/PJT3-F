# 알고리즘 활용 기록서

| 번호    | 알고리즘           | 요약                             | 비고               |
|---------|-------------------|----------------------------------|-------------------|
| Algo-01 | 운동 종목으로 관련 영상 검색 | 입력된 운동 종목 이름을 기반으로 관련 영상을 빠르게 검색한다. | 문자열 매칭 알고리즘(KMP) 적용 |
| Algo-02 | 조회수, 댓글수 정렬 기능 | 조회수나 댓글 수에 따라 영상을 정렬하여 사용자에게 제공한다. | 퀵 소트 또는 머지 소트 사용 |
| Algo-03 | 영상 추천 기능 | 사용자의 시청 기록을 바탕으로 관심 있을 만한 영상을 추천한다. | 사용자 선호 데이터 분석 활용 |
| Algo-04 | 자주 하는 질문 필터 | 입력된 질문 내용을 분석하여 자주 묻는 질문 카테고리로 자동 분류한다. | KMP 알고리즘을 이용한 텍스트 분석 |
| Algo-05 | 닉네임 변경하기 | 사용자가 원하는 닉네임의 중복 여부를 검사한다. | 라빈-카프 알고리즘을 사용하여 후보군 선별 후, KMP로 최종 확인 |




# 알고리즘 적용 기획서

## 1. 운동 종목으로 관련 영상 검색
- **알고리즘**: 문자열 매칭 알고리즘(KMP)
- **요약**: 사용자가 입력한 운동 종목 이름을 기반으로 관련된 영상을 검색한다.
- **이점**:
  - 검색 속도 향상: 효율적인 문자열 매칭 알고리즘을 사용하여 빠른 검색 결과 제공.
- **이슈사항**:
  - 문자열 정확도: 사용자의 입력 오류에 따른 검색 결과의 정확성 저하 가능성.

## 2. 조회수, 댓글수 정렬 기능
- **알고리즘**: 퀵 소트 또는 머지 소트
- **요약**: 사용자가 요청할 때마다 동적으로 영상 리스트를 조회수나 댓글 수에 따라 정렬한다.
- **이점**:
  - 사용자 맞춤형 콘텐츠 제공: 사용자가 선호할 가능성이 높은 콘텐츠를 우선적으로 제공.
- **이슈사항**:
  - 정렬 알고리즘 선정: 데이터 크기에 따른 최적의 정렬 알고리즘 선택 필요.

## 3. 영상 추천 기능
- **알고리즘**: 콘텐츠 기반 필터링 및 협업 필터링
- **요약**: 사용자의 시청 기록과 선호도를 분석하여 개인화된 영상을 추천한다.
- **이점**:
  - 사용자 경험 개선: 개인의 선호에 맞춰 맞춤형 콘텐츠를 제공, 시청 만족도 증가.
- **이슈사항**:
  - 데이터의 다양성과 충분성: 효과적인 추천을 위해 다양하고 충분한 양의 사용자 데이터 수집 필요.

## 4. 자주 하는 질문 필터
- **알고리즘**: KMP 문자열 매칭
- **요약**: 사용자가 입력한 질문을 분석하여 자주 발생하는 질문 카테고리를 자동으로 분류하고 답변을 제공한다.
- **이점**:
  - 고객 지원 효율성 증대: 자주 발생하는 질문에 대해 자동으로 답변함으로써 고객 지원 부담 감소.
- **이슈사항**:
  - 단어 인식 오류: 특정 키워드를 잘못 인식할 경우 잘못된 카테고리로 분류될 위험.

## 5. 닉네임 변경 기능
- **알고리즘**: 라빈-카프, KMP 문자열 매칭
- **요약**: 사용자가 원하는 닉네임을 입력할 경우, 먼저 라빈-카프 알고리즘으로 후보군을 선정하고, KMP 알고리즘으로 정확한 매칭을 확인한 후 중복 여부를 판단한다.
- **이점**:
  - 데이터 처리 효율성: 빠르고 효율적인 중복 검사를 통해 사용자 경험 개선.
- **이슈사항**:
  - 알고리즘 복잡도: 두 개의 문자열 매칭 알고리즘을 조합하여 사용함으로써 발생하는 복잡도 관리 필요.
