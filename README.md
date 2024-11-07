- Spring cloud config 사용할 때, 폴더 만들어서 거기 안에다가 파일 넣고 가져오는 거는 단순히 actuator만 가지고는 안 되는 것 같다.
- 아래 형식들만 가능한데, git의 branch 이름으로 폴더를 분기해야되나 싶다.
    /{application}/{profile}[/{label}]
    /{application}-{profile}.yml
    /{label}/{application}-{profile}.yml
    /{application}-{profile}.properties
    /{label}/{application}-{profile}.properties
- searchPath 라는 옵션을 사용해서 패턴 검색을 할 수가 있다.
    - 다만 actuator 경로 상에 폴더 이름을 넣을 수는 없을 것 같다.
    - 설정 파일들을 예쁘게 폴더 안에 넣어서 정리해 놓고 사용한다는 의의가 있겠다.