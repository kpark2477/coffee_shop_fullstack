# Coffee Shop Full Stack

## Project introduction

유다시티 full stack nanodegree 수업 authentification 프로젝트입니다.
Auth0 라는 3rd party 서비스를 이용하여, rs256 알고리즘을 활용한 인증과정을 적용하는 프로젝트입니다.
JWT를 활용하여 user별 다른 권한을 부여합니다.

프론트엔드는 유다시티에서 제공하고, 그에 맞추어 학생이 backend를 빌드하게 됩니다.

이 프로젝트는 간단한 cafe를 구현한 사이트입니다.
1) 각각의 음료별 재료의 비율을 그래픽적으로 디스플레이합니다.
2) 일반 유저도 음료의 이름과 그래픽을 볼수 있도록 허용합니다.
3) 바리스타는 레시피 정보를 확인할수 있는 권한이 있습니다.
4) 매니저는 새로은 음료를 추가하거나 기존 음료를 편집할 수 있습니다.

## How to run the servers

백엔드의 경우 python과 framework flask, sqlalchemy로 구축되어 있습니다.
프론트엔드의 경우 node와 framework ionic으로 구축되어 있습니다. 

각각의 readme 파일을 참고하시어, 백엔드 서버를 먼저 run 하시고, 프론트 엔드 서버를 run 해주세요.

1. [`./backend/`](./backend/README.md)
2. [`./frontend/`](./frontend/README.md)

## How to use the app

1. 처음 사이트를 여시면, 음료 4개와 해당 음료의 그래픽을 볼 수 있습니다. (일반유저의 권한은 여기까지입니다.)
2. 하단 메뉴에서 user를 클릭해서 user 페이지로 이동하면 바리스타나 매니저로 로그인할 수 있습니다.
(바리스타 ID barista@abc.com 비번 barista12!@ // 매니저 ID manager@abc.com 비번 manager12!@)
3. 로그인 하신 후 다시 하단 메뉴를 이용해서 drink 탭으로 이동하시면, 바리스타는 디테일한 레시피 확인이 가능하고,
메니저는 새음료 추가 및 삭제가 가능합니다.
4. 새음료 추가시에 재료 이름과 수량은 자유롭게 입력해주시고 컬러의 경우 blue, red, brown, yellow, black, white 등이 입력 가능합니다.
5. frontend가(유다시티에서 제공) 매끄럽지 않은 부분이 있습니다. 새음료를 추가하신 후에는 브라우저를 refresh 해주시고,
로그아웃시에 auth0 쿠키까지 로그아웃을 원하신다면
https://fsndq1.auth0.com/v2/logout?client_id=ffPxCY2qnnAi2YR8Vn3UN60uwPjW38T6&returnTo=http://localhost:8100/tabs/user-page
위의 링크를 눌러 로그아웃 해주십시오.
