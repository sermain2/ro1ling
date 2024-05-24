## 🖤 커밋 메시지 컨벤션

### 1. 커밋 유형 지정

- 커밋 유형은 영어 **소문자**로 작성한다.

  | 커밋 유형 | 의미                                                         |
  | --------- | ------------------------------------------------------------ |
  | feat      | 새로운 기능 추가                                             |
  | fix       | 버그 수정                                                    |
  | style     | 코드 formatting, 세미콜론 누락, 코드 자체의 변경이 없는 경우 |
  | refactor  | 코드 리팩토링                                                |
  | design    | CSS 등 사용자 UI 디자인 변경                                 |
  | test      | 테스트 코드, 리팩토링 테스트 코드 추가                       |
  | docs      | 문서 수정                                                    |
  | chore     | 패키지 매니저 수정, 그 외 기타 수정 ex) .gitignore           |
  | comment   | 필요한 주석 추가 및 변경                                     |
  | rename    | 파일 또는 폴더 명을 수정하거나 옮기는 작업만인 경우          |
  | remove    | 파일을 삭제하는 작업만 수행한 경우                           |
  | !HOTFIX   | 급하게 치명적인 버그를 고쳐야 하는 경우                      |

- Gitmogi 사용한다.

  - `npm i -g gitmoji-cli` 설치
  - 먼저 git add 명령어로 변경 사항을 스테이징
  - git commit -m 대신에 gitmoji -c 로 커밋메시지를 작성
  - 혹은 이모지 코드를 commit 명령어에서 사용할 수도 있음
  - 예시 : git commit -m ":sparkles: 검색 기능 추가”
  - [참고링크](https://inpa.tistory.com/entry/GIT-%E2%9A%A1%EF%B8%8F-Gitmoji-%EC%82%AC%EC%9A%A9%EB%B2%95-Gitmoji-cli)

  | 아이콘 | 코드                        | 설명                      |
  | ------ | --------------------------- | ------------------------- |
  | 🎨     | :art:                       | 코드의 구조/형태 개선     |
  | ⚡️    | :zap:                       | 성능 개선                 |
  | 🔥     | :fire:                      | 코드/파일 삭제            |
  | 🐛     | :bug:                       | 버그 수정                 |
  | ✨     | :sparkles:                  | 새 기능                   |
  | 📝     | :memo:                      | 문서 추가/수정            |
  | 💄     | :lipstick:                  | UI/스타일 파일 추가/수정  |
  | 🎉     | :tada:                      | 프로젝트 시작             |
  | ✅     | :white_check_mark:          | 테스트 추가/수정          |
  | 🔒     | :lock:                      | 보안 이슈 수정            |
  | 🔖     | :bookmark:                  | 릴리즈/버전 태그          |
  | ♻️     | :recycle:                   | 코드 리팩토링             |
  | ➕     | :heavy_plus_sign:           | 의존성 추가               |
  | ➖     | :heavy_minus_sign:          | 의존성 제거               |
  | 🔧     | :wrench:                    | 구성 파일 추가/삭제       |
  | 🔨     | :hammer:                    | 개발 스크립트 추가/수정   |
  | 💩     | :poop:                      | 똥싼 코드                 |
  | ⏪     | :rewind:                    | 변경 내용 되돌리기        |
  | 🔀     | :twisted_rightwards_arrows: | 브랜치 합병               |
  | 👽     | :alien:                     | 외부 API 변화로 인한 수정 |
  | 💡     | :bulb:                      | 주석 추가/수정            |
  | 🙈     | :see_no_evil:               | .gitignore 추가/수정      |

### 2. 제목과 본문을 빈행으로 분리한다.

- 커밋 유형 이후 제목과 본문은 한글로 작성하여 내용이 잘 전달될 수 있도록 할 것
- 본문에는 변경한 내용과 이유 설명 (어떻게보다는 무엇 & 왜를 설명)

### 3. 제목 첫 글자는 소문자로, 끝에는 `.` 쓰지 않는다.

### 4. 제목은 한글 50자 이내로 한다.

### 5. 자신의 코드가 직관적으로 바로 파악할 수 있다고 생각하지 말자.

### 6. 여러가지 항목이 있다면 글머리 기호를 통해 가독성 높인다.

```
- 변경 내용 1
- 변경 내용 2
- 변경 내용 3
```

</aside>

### 🖤 규칙에 맞는 좋은 커밋메시지를 작성해야 하는 이유

- 팀원과의 소통
- 편리하게 과거 추적 가능
- 나중에 실무에서 익숙해지기 위해

### 🖤 한 커밋에는 한 가지 문제만!

- 추적 가능하게 유지해주기
- 너무 많은 문제를 한 커밋에 담으면 추적하기 어렵다.

### 🖤 CLI에서 커밋 메시지 여러 줄로 작성하는 방법

- 쌍따옴표를 닫지 말고 개행하며 작성 → 다 작성한 후에 쌍따옴표를 닫으면 작성 완료

  ```bash
  git commit -m "FEAT: 회원가입 기능 추가

  - 회원가입 기능 추가"-
  ```