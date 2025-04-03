```mermaid
flowchart LR
    A[시작] -->|불량, 합격 이미지 준비| B[AI 모델 데이터 학습]
    B -->|파이썬 코드 작성| C[OpenVINO 추론 모듈 실행]
    C -->|추론 결과| D[나사 체결상태 불량, 합격 구분]
    D -->|결과 출력| E[video capture화면에 표시]




```mermaid
flowchart LR
    A[입력 데이터] -->|전처리| B[모델 A 추론]
    A -->|전처리| C[모델 B 추론]
    B -->|결과| D[출력 A]
    C -->|결과| E[출력 B]
