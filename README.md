```mermaid
flowchart LR
    A[시작] -->|불량, 합격 이미지 준비| B[AI 모델 데이터 학습]
    B -->|파이썬 코드 작성| C[OpenVINO 추론 모듈 실행]
    C -->|추론 결과| D[나사 체결상태 불량, 합격 구분]
    D -->|결과 출력| E[video capture화면에 표시]
    D -->|결과 출력| F[PLC로 신호 전달]
