# A1 리포트

- 이름: 김권섭
- 학번: 2023202024
- GitHub ID: kwonseop

## 어디를 둘러봤는지

awesome-nodejs의 Command-line utilities 카테고리를 둘러보았다.
터미널에서 `npm search "terminal spinner"`를 검색하여 터미널에서 사용할 수 있는 패키지들을 찾아보았다.

또한 터미널에서 `npm search dayjs`를 검색하여 날짜와 시간을 다루는 패키지들을 살펴보았다.

마지막으로 터미널에서 `npm search "cli table"`을 검색하여 터미널에서 표를 출력할 수 있는 패키지들을 살펴보았다.

---

## 선정한 패키지

### 1. `ora`

**선정 이유:**
터미널에서 로딩 상태를 보여줄 수 있다는 점이 신기하게 다가왔고 프로그램이 실행중이란 것을 시각적으로 보여주기에 유용하다고 생각돼서 선택하게 되었다.

**이것으로 무엇을 할 수 있을지:**
시간이 오래 걸리는 작업에서 로딩 상태를 보여주는 프로그램에 이용할 수 있을 것 같다. 또한 작업이 종료됐을 때 성공/실패 여부 등을 표시하여 진행 상태를 확인하는 것에 도움을 줄 수 있을 것 같다.

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

**출력을 보고 알게 된 것:**
현재 버전은 9.4.1이고 메타데이터가 2026년 6월에 수정된 것을 확인했다.
또한 deprecated 명령에서 아무것도 출력되지 않았기 때문에 현재도 관리되고 있는 패키지라고 생각한다.

---

### 2. `dayjs`

**선정 이유:**
날짜와 시간을 계산하거나 원하는 형식으로 쉽게 바꿀 수 있다는 점이 실용적으로 다가와 궁금해서 선택했다.

**이것으로 무엇을 할 수 있을지:**
과제나 특정 이벤트의 마감일까지 며칠이 남았는지 계산해주는 프로그램을 만들 수 있을 것 같다.
또 날짜와 시간을 원하는 형식으로 변환하여 일정이나 기록을 보기 쉽게 출력하는 프로그램에 사용할 수 있을 것 같다.

**확인 결과:**

```
$ npm view dayjs version time.modified license dependencies
version = '1.11.23'
time.modified = '2026-08-17T11:52:35.546Z'
license = 'MIT'
$ npm view dayjs deprecated
```

**출력을 보고 알게 된 것:**
현재 버전은 1.11.23이고 메타데이터가 2026년 8월에도 수정된 것을 확인했다.
또한 deprecated 명령에서 아무것도 출력되지 않았고 별도의 dependencies도 출력되지 않아, 의존 패키지 없이 사용할 수 있으며 지원이 중단된 패키지도 아닌 것으로 확인했다.

---

### 3. `cli-table3`

**선정 이유:**
터미널에서도 데이터를 표 형태로 깔끔하게 정리해서 보여준다는 것을 보고 어떻게 보이게 될지 궁금하여 선택했다.

**이것으로 무엇을 할 수 있을지:**
데이터들을 터미널에서 보기 좋은 표 형태로 출력하는 프로그램을 만들 수 있을 것 같다.
또한 여러 항목을 행과 열로 구분해서 표현하는 것에 응용할 수 있을 것 같다.

**확인 결과:**

```
$ npm view cli-table3 version time.modified license dependencies
version = '0.6.5'
time.modified = '2024-05-12T16:36:50.251Z'
license = 'MIT'
dependencies = { 'string-width': '^4.2.0' }
$ npm view cli-table3 deprecated
```

**출력을 보고 알게 된 것:**
현재 버전은 0.6.5이고 npm search 결과를 통해 2024년 5월에 배포된 버전이라는 것을 확인했다.
최근 몇 년 동안 새로운 버전이 배포되지는 않았지만 deprecated 상태는 아닌 것을 알 수 있었다.

---

## 설치해본 패키지

```
$ npm install ora

added 17 packages, and audited 18 packages in 616ms

17 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities

$ node try.js
⠹ 작업 중 !
✔ 작업 완료 !

```

---

## 막혔던 부분 (채점하지 않음)

에러 메시지든 헷갈렸던 부분이든 하나. 두 문장이면 됩니다. 없었으면 없었다고 적습니다.

```
이런 패키지를 설치부터 실행까지 하는 일련의 과정 자체가 처음이어서 초반엔 어색했습니다.
```

---

## AI 사용

사용 프롬프트 : ora 패키지를 설치하는 일련의 과정들을 자세하게 알려줘
잘못된 정보는 없었습니다.

---

## 제출 전 확인

- [ ] 저장소 이름이 `oss2026-a1`, 공개 범위가 Public
- [ ] `git status` 결과가 `nothing to commit, working tree clean`
- [ ] `node_modules` 폴더를 지우고 `npm install` → `node try.js` 를 다시 해도 실행됨
- [ ] 마지막 커밋을 push함
