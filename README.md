```mermaid
flowchart LR
    시작([시작])
    시작-->|Train 데이터준비| --> Yolo 모델 구축
    시작-->|코드작성| --> 코드 검토

    시작 --> Yolo[YOLO 모델 구축]
    시작 --> 코드검토[코드검토]

    Yolo --> 실행[프로그램 실행]
    코드검토 --> 실행

    실행 --> 검토[검토]
    검토 --> Yolo
    검토 --> 코드검토

    검토 --> 정리[필요 요소 정리]
    정리 --> 도커[도커라이징]
    도커 --> 종료([종료])

    %% 설명용 보조 노드
    데이터준비[[Train 데이터 준비]]
    코드작성[[파이썬 코드 작성]]
```
