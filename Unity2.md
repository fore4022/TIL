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