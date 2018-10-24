# xairc 오픈소스 프로젝트 가이드라인

이 저장소(Repository)는 xairc GitHub 그룹에 포함되는 저장소를 대상으로 오픈소스 개발방법에 대한 가이드라인을 제공하는 것이 주 목적이며, 이를 통해 그룹 내에 있는 모든 오픈소스 프로젝트들의 효과적인 오픈소스 개발을 장려하고 전체적으로 어느 정도 통일된 규칙을 적용하여 서로 간의 소통을 원활히 하고자 합니다. xairc 그룹에 프로젝트를 업로드하기 전에 여기에서 다루고 있는 조치들을 취했는지 확인하는 것을 권장합니다.

&nbsp;

## 문서 작성

xairc 그룹 내의 모든 오픈소스 프로젝트는 저장소 안에 반드시 다음과 같은 문서 파일들을 포함하고 있어야 합니다. 라이선스 파일을 제외한 모든 문서는 마크다운 (Markdown)으로 작성하는 것을 원칙으로 합니다.

- `LICENSE`
- `README.md` 
- `CONTIRBUTING.md` (기여방법 가이드라인)
- `CODE_OF_CONDUCT` (행동 규약)

&nbsp;

### LICENSE 선택

모든 프로젝트는 새 오픈소스 프로젝트를 생성할 때 라이선스를 선택해야 합니다. 프로젝트에 어떤 라이선스가 적용되어 있는지 명시하기 위해 LICENSE 파일을 각 라이선스에 맞게 선택하여 추가하여야 합니다. 각 라이선스들은 이에 해당하는 규약들이 적힌 문서인 `LICENSE` 파일을 제공합니다. 이 파일은 GitHub 프로젝트를 생성할 때 함께 생성하거나 라이선스 페이지들로부터 복사해서 사용할 수 있습니다. 자주 사용되는 라이선스들은 MIT, Apache 2.0, GPLv3 등이 있습니다. 각 프로젝트의 목적에 따라 알맞은 라이선스를 선택해서 사용하면 됩니다.

- MIT License : 상업적 사용, 수정, 배포 등을 허가하지만 어떠한 형태의 법적 보증 또는 책임을 지지 않음
- GNU GPL (General Public License) v3 : 
  어떠한 목적으로도 사용, 수정할 수 있지만 이 라이선스가 포함된 소프트웨어의 일부라도 사용했다면 반드시 공개 배포해야 하며, 똑같은 라이선스를 사용해야 함
- Apache 2.0 : 이 라이선스가 포함된 소프트웨어를 수정한 경우에도 소스코드를 공개할 의무는 없지만 똑같은 라이선스를 사용해야 함

&nbsp;

### README 작성

README는 기본적으로는 프로젝트 사용방법 및 프로젝트의 목표에 대해서 서술하는 문서입니다. 또한 README는 프로젝트에 대해 다음 질문에 답할 수 있게 작성되어야 합니다.

- 이 프로젝트는 무엇을 하는가?
- 이 프로젝트는 왜 유용한가?
- 이 프로젝트를 사용하려면 가장 먼저해야 할 일은 무엇인가?
- 이 프로젝트와 관련해 더 많은 도움을 받으려면 어떻게 해야 하는가?

&nbsp;

### `CONTRIBUTING.md` 작성

기여방법 가이드라인 (Contributing Guideline)이란 프로젝트에 참여하고 싶어하는 기여자(Contributor)들에게 이 프로젝트에 참여할 수 있는 방법과 규칙을 명시해주는 문서입니다. 이 문서는 마크다운 문서인 `CONTRIBUTING.md` 파일로 작성합니다. 이 문서는 다음과 같은 기술적 정보를 포함해야 합니다.

- 커밋 (commit) 단위 및 작성 규칙
- 이슈 (Issue) 및 풀리퀘스트(Pull-Request), 버그 리포트를 제출하는 방법
- 새로운 기능(feature)을 제안하는 방법
- 환경설정 및 테스트 실행 방법

&nbsp;

위와 같은 기술적인 세부사항 외에도 `CONTRIBUTING.md` 는 프로젝트에서 다른 기여자들로부터 어떤 기여를 받고 싶어하는 지에 대한 정보를 전달할 수 있는 문서입니다. 따라서 다음 정보를 추가적으로 포함시킬 수 있습니다.

- 프로젝트에서 원하는 기여의 종류
- 프로젝트의 로드맵 및 비전
- 기여자(contributor)가 관리자(maintainer)에게 연락할 수 있는 방법

이 프로젝트에 있는 `CONTRIBUTING.md` 파일은 이 문서를 작성하기 위한 템플릿입니다. ([출처](https://github.com/nayafia/contributing-template/blob/master/CONTRIBUTING-template.md)) 다음과 같은 다른 대규모 프로젝트들의 `CONTRIBUTING.md`를 참고하는 것도 좋을 것입니다.
ex) [Tensorflow](https://github.com/tensorflow/tensorflow/blob/master/CONTRIBUTING.md),  [Atom](https://github.com/atom/atom/blob/master/CONTRIBUTING.md), [node.js](https://github.com/nodejs/node/blob/master/CONTRIBUTING.md), ...

&nbsp;

### `CODE_OF_CONDUCT.md` 작성 

행동규약 (Code of Conduct) 이란 프로젝트에 참여하는 사람들이 지켜야할 의무와 행동규칙에 대해서 규정하는 문서입니다. 이는 건강하고 건설적인 커뮤니티 분위기 조성을 위한 것으로 이 문서에는 참여자들이 해야 할 행동과 하지 말아야 할 행동과 그것을 위반했을 때 어떠한 조치를 취할 것인지에 대한 규칙을 명시하도록 합니다. 행동규약은 마크다운 문서인 `CODE_OF_CONDUCT.md` 파일로 작성합니다. 이 문서는 다음과 같은 내용들이 우선적으로 포함되어 있어야 합니다.

- 행동규약의 효력의 범위 (Issue, Pull Request, Event 같은 커뮤니티에 한정되는지 등)
- 행동규약이 적용되는 대상 (커뮤니티 멤버나 관리자에 한하는 지 등)
- 행동규약을 위반하면 했을때 어떤 조치를 취하는가? (해당 기여자의 프로젝트 참여 일시금지, 영구금지 등)
- 행동규약을 위반사항을 발견했을때 어떻게 신고하는가? 

이 프로젝트에 있는 `CODE_OF_CONDUCT.md` 파일은 [Contributor Covenant](https://www.contributor-covenant.org/version/1/4/code-of-conduct.html)에서 제공하는 행동규약의 예시 파일입니다. 위 링크에 있는 프로젝트들의 저장소에서도 같은 파일들을 예제로 찾아볼 수 있습니다.

&nbsp;

## 체크리스트

오픈소스 프로젝트를 xairc 그룹에 올리기 전에, 아래와 같은 체크리스트를 모두 만족시키는지 확인해야 합니다.

**문서**

- [ ] 프로젝트에 오픈소스 라이선스가 있는 `LICENSE` 파일이 있는가?
- [ ] 프로젝트에 위에서 언급한 문서가 있는가? (`README.md`, `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`)

**코드**

- [ ] 프로젝트가 일관된 코드 컨벤션(convention)을 사용하고 있는가?
- [ ] 함수/메소드/변수 이름이 사용목적과 일치하게끔 명확히 선언되었는가?
- [ ] 코드에 부가적인 설명이 필요한 경우 그 의도를 설명하기 위해 주석을 사용했는가?
- [ ] 버전관리 기록, 이슈, 혹은 pull requests에 민감한 데이터가 포함되지 않았는가? (예, 비밀번호 등 개인정보)

&nbsp;

### References

- GitHub Starting an Open Source Project (https://opensource.guide/starting-a-project/)

- License 종류 (http://www.bloter.net/archives/209318)

- CONTRIBUTING.md Template (https://github.com/nayafia/contributing-template/blob/master/CONTRIBUTING-template.md)

- Contributor Covenant (https://www.contributor-covenant.org/version/1/4/code-of-conduct.html)
