# A1 리포트

- 이름: 김권섭
- 학번: 2023202024
- GitHub ID: kwonseop

## 어디를 둘러봤는지

awesome-nodejs의 Command-line utilities 카테고리를 둘러보았다.
터미널에서 `npm search "terminal spinner"`를 검색하여 터미널에서 사용할 수 있는 패키지들을 찾아보았다.

---

## 선정한 패키지

### 1. `ora`

**선정 이유:
터미널에서 로딩 상태를 보여줄 수 있다는 점이 신기하게 다가왔고 프로그램이 실행중이란 것을 시각적으로 보여주기에 유용하다고 생각돼서 선택하게 되었다.**

**이것으로 무엇을 할 수 있을지:
시간이 오래 걸리는 작업에서 로딩 상태를 보여주는 프로그램에 이용할 수 있을 것 같다.
또한 작업이 종료됐을 때 성공/실패 여부 등을 표시하여 진행 상태를 확인하는 것에 도움을 줄 수 있을 것 같다.
**

**확인 결과:**

```
$ npm view ora version time.modified license dependencies
version = '9.4.1'
time.modified = '2026-06-22T12:24:49.363Z'
license = 'MIT'
dependencies = {
  chalk: '^5.6.2',
  'cli-cursor': '^5.0.0',
  'cli-spinners': '^3.2.0',
  'is-interactive': '^2.0.0',
  'is-unicode-supported': '^2.1.0',
  'log-symbols': '^7.0.1',
  'stdin-discarder': '^0.3.2',
  'string-width': '^8.1.0'
}

$ npm view ora deprecated

```

**출력을 보고 알게 된 것:
현재 버전은 9.4.1이고 데이터가 2026년 6월에 수정된 것을 확인했다.
또한 deprecated 명령에서 아무것도 출력되지 않았기 때문에 현재도 관리되고 있는 패키지라고 생각한다.
**

---

### 2. `<패키지이름>`

**선정 이유:**

**이것으로 무엇을 할 수 있을지:**

**확인 결과:**

```

```

**출력을 보고 알게 된 것:**

---

### 3. `<패키지이름>`

**선정 이유:**

**이것으로 무엇을 할 수 있을지:**

**확인 결과:**

```

```

**출력을 보고 알게 된 것:**

---

## 설치해본 패키지

```
$ npm install <패키지이름>

$ node try.js

```

---

## 막혔던 부분 (채점하지 않음)

에러 메시지든 헷갈렸던 부분이든 하나. 두 문장이면 됩니다. 없었으면 없었다고 적습니다.

```

```

---

## AI 사용

사용했다면 프롬프트와, AI의 설명이 실제와 달랐던 부분을 적습니다.
사용하지 않았다면 "사용하지 않음"이라고만 적으면 됩니다.

---

## 제출 전 확인

- [ ] 저장소 이름이 `oss2026-a1`, 공개 범위가 Public
- [ ] `git status` 결과가 `nothing to commit, working tree clean`
- [ ] `node_modules` 폴더를 지우고 `npm install` → `node try.js` 를 다시 해도 실행됨
- [ ] 마지막 커밋을 push함
