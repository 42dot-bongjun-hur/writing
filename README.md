# Writing Blog Starter

짧은 관찰형 글과 한 장의 단순한 삽화를 만드는 최소 구성이다.

핵심은 두 종류의 정보를 섞지 않는 것이다.

- `guides/`: 모든 글에 공통으로 적용되는 규칙
- `golden/`: 사람의 입력과 사람이 승인한 결과의 쌍

## 구조

```text
writing-blog-starter/
├── README.md
├── guides/
│   ├── AGENT.md
│   ├── WRITING.md
│   └── ILLUSTRATION.md
├── golden/
│   └── _TEMPLATE.md
└── drafts/
```

## 무엇을 어디에 둘까

### guides/

한 번 정하면 모든 글에 적용되는 규칙을 둔다.

예:

- 문장은 짧게 쓴다.
- 장면을 먼저 보여준다.
- 독자를 훈계하지 않는다.
- 삽화는 검은 손선과 한 가지 포인트 색을 사용한다.
- 그림 안에 텍스트를 넣지 않는다.

같은 지시가 여러 글에서 반복되면 Golden Example에 계속 적지 말고 Guide로 승격한다.

### golden/

특정 입력에 대해 “이 결과를 정답으로 본다”는 승인 데이터만 둔다.

필수:

- `Source`: 사람이 준 원재료
- `Final`: 사람이 승인한 최종 글

선택:

- `Illustration`: 이 글에서 특별히 그리고 싶은 장면이 있을 때만
- `Note`: 이 글에서만 중요한 예외나 편집 피드백이 있을 때만

`Illustration`과 `Note`가 없으면 정상이다. Agent가 Global Guide에 따라 알아서 처리한다.

## 가장 중요한 규칙

**모든 글에 적용되면 Guide. 이 글에서만 필요하면 Golden Example.**

Golden Example은 프롬프트가 아니다. 입력과 승인된 출력의 쌍이다.

## 운영 흐름

```text
사람의 메모
  -> Agent 초안
  -> 사람이 수정/승인
  -> golden/ 에 저장
  -> 다음 글의 참고 데이터가 됨
```

승인되지 않은 글은 `golden/`에 넣지 않는다.
