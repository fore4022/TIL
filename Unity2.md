# Unity 2
# C#
* raycasthit2d : raycast를 통해서 충돌 정보를 담는 구조체
    * bool collider : 충돌 객체의 콜라이더 유무
    * collider2d collider2d : 충돌 객체의 collider2d 컴포넌트 참조
    * transform transform : 충돌 객체의 transform 컴포넌트 참조
    * vector2 point : 충돌 지점 좌표
    * vector2 noraml : 충돌 객체의 법선 벡터
    * float distance : 충돌 지점까지 거리
* spherecast : 구 형태의 충돌 영역을 가진 raycast
    * origin : 출발점의 위치 지정 vector3 변수
    * radius : 구체의 반지름을 나타낸 보동소수점 변수
    * direction : ray 방향을 나타내는 vector3 변수
    * hitinfo : 충돌 정보 저장 raycasthit 변수
    * maxdistance : ray 최대 길이를 지정하는 부동소수점 변수
* layer : 게임 오브젝트를 그붑화하고, 여려개의 layer에 속할 수 있다
* tag : 오브젝트를 식별하는데 사용된다, 오브젝트당 하나의 tag를 가진다
* rigidbody2d.velocity : rigidbody2d가 적용된 게임 오브젝트의 속도 vector를 나타낸다, 속도 vector의 값은 실제 게임 오브젝트의 이동 방향과 동일하다
* moveposition : rigidbody 컴포넌트에서 제공되며, 오브젝트의 위치를 지정된 위치로 부드럽게 이동시킨다, 이동시킬때 선형 보간을 하여 이동시켜서, 물리 시뮬레이션과 관련 없이 곧 바로 오브젝트를 이동시킨다
* <oncollision enter, stay, exit은 collider를 가진 2개의 객체 중에서 한개의 객체가 움직이고 있는 상태여야지만 실행이 된다, 이와 같은 이유는 충돌에 관련된 최적화를 위한 설계이자, 시뮬레이션의 성능을 향상시키기 위해서이다>