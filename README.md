```mermaid
flowchart LR
    A[아두이노 제어 코드] -->|직렬 통신| B[아두이노 장치]
    B -->|데이터 전송| C[OpenVINO 추론 모듈]
    C -->|추론 결과| D[캠1 모양 인식]
    D -->|결과 출력| E[터미널/GUI]
