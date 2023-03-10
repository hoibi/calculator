# calculator
git 실습을 위한 저장소입니다.

.gitignore
    - 빌드 결과물 혹은 임시 파일 등은 굳이 버전관리 할 필요가 없다
    - 이런 파일들은 Stage에 추가하지 않는 식으로 관리할 수도 있겠지만 git이 해당 파일들을 무시하도록 할 수 있습니다.
    - .gitignore라는 텍스트 파일을 만들어서 한줄 씩 무시할 파일 이름의 패턴을 적어주면 됩니다.
    - https://www.gitignore.io/
        - 주요 운영체제, 언어에 대한 .gitignore패턴을 자동으로 생성해주는 사이트

    이미 버전 관리된 파일을 무시하기
    - 이미 커밋되어 버전관리가 되는 파일은 이후에 .gitignore에 추가해도 무시되지 않습니다.
    - 이 경우 해당 파일을 삭제한 후 커밋하고해야 합니다
        - 무시할 파일의 경우 저장소에 들어 있지 않아도 빌드 과정에서 다시 만들어지는 파일이므로 삭제해도 무방합니다.

브랜치
    - 브랜치란 가상의 작업 공간
    - 브랜치를 왜 만들고 사용해야 하는지 알아 봅시다
    - 실제 개발 과정에서 겪을 만한 예제.
        1. 작업 중인 웹사이트가 있다.
        2. 새로운 이슈를 처리할 새 브랜치를 하나 생성한다.
        3. 새로 만든 브랜치에서 작업을 진행한다.
    - 중요한 문제가 생겨서 해결하는 hotfix를 만들어야 한다면
        1. 새로운 이슈를 처리하기 전의 운영 브랜치로 이동한다.
        2. hotfix 브랜치를 새로 생성한다
        3. 수정한 hotfix 테스트를 마치고 운영 브랜치로 머지한다
        4. 다시 작업하던 브랜치로 옮겨가서 하던 일을 진행한다.