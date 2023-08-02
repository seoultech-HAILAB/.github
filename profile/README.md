## Welcome to HAILAB GITHUB! 👋

more information : https://hai.seoultech.ac.kr/
<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->

# HAILAB Coding Rule 규칙
- 다음 `Coding Rule` 하위 내용을 각 프로젝트(Repository) 마다 복사하여 작업해주세요.
- 본 `Coding Rule`은 각 프로젝트 사정에 맞게 수정하여 사용할 수 있습니다.

>문의 : [DY-76](https://github.com/DY-76)
# Coding Rule
> 제정 23.2
> 개정 23.4
> 개정 23.8
- 작업, 유지보수의 편의성 증진과 효율적이고 강건한 애플리케이션 개발을 위해 `Coding Rule`을 제정한다.
## Naming
- Class = `PascalCase`
- variable, function, method = `camelCase`
- constant variable = `UPPER_CASE`
- filename, folder = `kebab-case`
## Modulization
## 개발 방법론
## Branch Naming
- `master`(main, origin etc...)
  - `master branch`는 `Repository` 생성시 자동으로 생성된다.
  - 일반적으로 완성된 최신 작업물을 `merge`하는 곳으로 사용한다.
  - `feature branch`에서 `PR`을 받아 책임 혹은 담당 개발자가 검토 후 `merge`한다.
- `develop`
  - `develop branch`는 애플리케이션의 개발을 진행할 때 사용한다.
  - 일반적으로 `develop/담당자식별-목표Version` 형식을 추천한다. ex) develop/LDY-1.2 등
  - 작업이 완료된 경우, `master branch`로 `PR`을 보내고 정상적으로 `merge`된 경우 제거한다.
- `feature`
  - `feature branch`는 애플리케이션의 기능을 제작할 때 사용한다.
  - 일반적으로 `feature/기능이름` 형식을 추천한다. ex) feature/login 등
  - 작업이 완료된 경우, `develop branch`로 `PR`을 보내고 정상적으로 `merge`된 경우 제거한다.
- `release`
  - `release branch`는 애플리케이션을 배포할 때 사용한다.
  - 일반적으로 `release/Version` 형식을 추천한다. ex) release/1.2 등
  - 특정 시점의 작업이 완료된 `Master branch`에서 배포하고자 하였을 때 `release branch`를 생성하고 더이상 작업하지 않는다(기록용 branch).
- `hotfix`
  - `hotfix branch`는 애플리케이션의 오류를 수정할 때 사용한다.
  - 일반적으로 `hotfix/Version.num` 형식을 추천한다. ex) hotfix/1.2.2 등
  - 작업이 완료된 경우, `master branch`, `feature branch`로 `PR`을 보낸다.
