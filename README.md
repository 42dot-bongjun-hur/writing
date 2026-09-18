# Writing Blog Starter

짧은 관찰형 글과 한 장의 단순한 삽화를 한 세트로 만드는 블로그용 콘텐츠 시스템이다.

이 저장소는 **아이디어 메모 → 글 작성 → 편집 → 삽화 브리프 → 발행** 흐름을 반복 가능하게 만드는 것을 목표로 한다. 특정 주제에 묶이지 않으며, 기술·일·관계·학습·일상 경험을 같은 문법으로 다룰 수 있다.

## 핵심 원칙

1. 한 문단에는 하나의 생각만 둔다.
2. 추상적인 주장보다 사람이 겪는 장면을 먼저 쓴다.
3. 문장은 짧고 단정하게 쓴다.
4. 의미는 설명으로 밀어 넣지 않고, 장면 뒤에서 드러나게 한다.
5. 마지막 문장은 앞 내용을 요약하기보다 한 단계 추상화한다.
6. 삽화는 글 전체를 설명하지 않는다. 핵심 개념이 드러나는 장면 하나만 그린다.
7. 글과 그림 모두 여백을 남긴다.

## 폴더 구조

```text
writing-blog-starter/
├── README.md
├── AGENT_SYSTEM_PROMPT.md
├── STYLE_GUIDE.md
├── CONTENT_MODEL.md
├── ILLUSTRATION_GUIDE.md
├── WORKFLOW.md
├── CHECKLIST.md
├── config/
│   └── blog-style.yaml
├── templates/
│   ├── idea-note.md
│   ├── post.md
│   └── illustration-brief.md
├── prompts/
│   ├── 01_from_note_to_structure.md
│   ├── 02_write_post.md
│   ├── 03_edit_post.md
│   └── 04_make_illustration_brief.md
├── examples/
│   └── firmware-debugging.md
├── references/
│   └── style_reference.png
└── content/
    ├── drafts/
    └── published/
```

## 가장 먼저 쓸 파일

- 에이전트에 넣을 프롬프트: `AGENT_SYSTEM_PROMPT.md`
- 사람이 읽는 전체 문체 기준: `STYLE_GUIDE.md`
- 삽화 기준: `ILLUSTRATION_GUIDE.md`
- 새 글 시작: `templates/idea-note.md`
- 최종 글 형식: `templates/post.md`

## 권장 사용 흐름

1. `templates/idea-note.md`에 떠오른 경험을 거칠게 적는다.
2. `prompts/01_from_note_to_structure.md`로 글의 중심 장면과 문단 구조를 잡는다.
3. `prompts/02_write_post.md`로 초안을 만든다.
4. `prompts/03_edit_post.md`로 군더더기를 덜어낸다.
5. `prompts/04_make_illustration_brief.md`로 삽화 장면을 만든다.
6. `CHECKLIST.md`를 통과하면 `content/published/`로 옮긴다.

## 한 문장으로 정의

**장면을 먼저 보여주고, 의미는 나중에 남기는 짧은 글과 여백 많은 한 장의 삽화.**
