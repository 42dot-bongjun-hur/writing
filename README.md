# Writing Blog Starter

짧은 관찰형 글과 한 장의 단순한 삽화를 한 세트로 만드는 블로그용 콘텐츠 시스템이다.

이 저장소는 **아이디어 메모 -> 글 구조 -> 초안 -> 편집 -> 삽화 브리프 -> 발행** 흐름을 반복 가능하게 만든다.
기술, 일, 관계, 학습, 일상 경험을 같은 문법으로 다룰 수 있다.

## 핵심 원칙

1. 한 문단에는 하나의 생각만 둔다.
2. 추상적인 주장보다 사람이 겪는 장면을 먼저 쓴다.
3. 문장은 짧고 단정하게 쓴다.
4. 의미는 장면 뒤에서 드러나게 한다.
5. 삽화는 글 전체를 설명하지 않고 핵심 장면 하나만 그린다.
6. 그림은 특정 레퍼런스를 그대로 복제하지 않는 독립적인 `Note Cartoon` 하우스 스타일을 쓴다.

## 폴더 구조

```text
writing-blog-starter/
├── README.md
├── AGENT_SYSTEM_PROMPT.md
├── STYLE_GUIDE.md
├── VISUAL_IDENTITY.md
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
│   └── REFERENCE_POLICY.md
└── content/
    ├── drafts/
    └── published/
```

## 먼저 볼 파일

- 에이전트에 바로 넣을 프롬프트: `AGENT_SYSTEM_PROMPT.md`
- 글 문체 기준: `STYLE_GUIDE.md`
- 그림의 브랜드 방향: `VISUAL_IDENTITY.md`
- 실제 삽화 생성 규칙: `ILLUSTRATION_GUIDE.md`
- 새 글 시작: `templates/idea-note.md`
- 발행 전 확인: `CHECKLIST.md`

## 권장 사용 흐름

1. `templates/idea-note.md`에 경험을 거칠게 적는다.
2. `prompts/01_from_note_to_structure.md`로 중심 장면과 문단 구조를 잡는다.
3. `prompts/02_write_post.md`로 초안을 만든다.
4. `prompts/03_edit_post.md`로 군더더기를 덜어낸다.
5. `prompts/04_make_illustration_brief.md`로 삽화 장면을 만든다.
6. `ILLUSTRATION_GUIDE.md`와 `VISUAL_IDENTITY.md`로 그림을 생성한다.
7. `CHECKLIST.md`를 통과하면 `content/published/`로 옮긴다.

## 하우스 스타일 한 문장

**짧은 관찰문과, 조금 삐뚤고 단순한 검은 손선에 한 가지 색만 얹은 노트 카툰.**
