# Unity 1
# C#
* enum : 상수 열거형
* struct : 구조체
* ref, out : 변수에 입력되는 값을 원본으로 입력해주거나, 결과를 out을 통해 반환
* class : 각 객체를 생성하기 위한 템플릿
* 디버깅 : 실행되는 중간 과정을 확인해 보면서 값을 수정할 수 있고, 이전 상황으로 진행 상황을 되돌리며, 실행 중간에 멈추게 할 수 있음
* queue : 선입선출 자료구조
    * enqueue : queue에 요소 추가
    * dequeue : queue에 가장 앞 요소를 제거하고 반환
* info : 객체에 대한 정보를 포함하는 데이터(실제론 info 객체는 a 메서드에 정의된 속성과 메소드 사용해 정보 처리, 반환 할수 있다)
* var : 초기화 값으로 자동으로 타입을 추론해 사용하도록 함
* yield return : 메서드, 이터레이터(컬렉션을 순회나 반복 처리 기능)블록의 값을 반환하며, 실행을 일시 중단
    * yield return null : 다음 프레임까지 대기
    * yield return new waitforseconds : 지정된 시간 만큼 대기
    * yield return new waituntil : 주어진 조건이 참이 될때까지 코루틴의 실행을 질시 중지하는 명령
* enumerator : 컬렉션을 반복하는데 사용, 컬렉션의 요소를 하나씩 차례로 검색하여, 모든 요소에 접근
* foreach : 반복문을 수행하는 구문, 데이터 집합 요소를 하나씩 가져와 반복작업을 수행
* euler : 3개의 각도로 이루어진 좌표계
* play : 파티클 재생 메서드로, 파티클 시스템 시작 또는 중단된 파티클 재생
* minmaxcurve : 파티클 모듈에서의 값, min과 max의 값을 가지며, 시간에 따라 값이 변하는 그래프를 만드려고 사용함
* comparetag : 현재 오브젝트의 tag와 주어진 문자열 tag를 비교해 반환한다
* identity : 객체 식별에 사용
* private : 선언한 해당 클래스에서만 사용이 가능하며, 해당 클래스의 메서드를 통해야 변수에 접근할 수 있다
* meterial : 각각의 renderer컴포넌트마다, meterial속성을 가질 수 있다, 정의된 속성을 가지며, rendering의 색, 반사율, 텍스처 매핑을 조작
* lerp : 선형 보간, 시작 색상과 목표 색상을 설정하여 두가지 색상 사이의 중간 색상을 생성 가능
* particle collision : 파티클 시스템의 충돌을 구현할 때 사용
    * enable dynamic colliders : 파티클이 움직일 때 동적으로 충돌 판정
    * collider force : 파티클 충돌기반으로 가하는 힘
    * bounce : 충돌 시 튕김 효과
    * radius scale : 값을 조절해 충돌 범위 조절
    * visualize bounds : 파티클 시스템 충돌 경계 시각화
    * collides with : 충돌 판정을 수행할 대상 지정
* Debug : 디버깅과 로그 출력 클래스
    * log : 로크를 출력해 콘솔 창에 표시한다
    * logwarning : 콘솔에 표시 되는 경고 메세지 출력
    * logerror : assert메서드를 사용해 조건 확인, 참일 경우 디버깅 종료
* navmesh : 이동가능 지역정의, 이동 가능 영역을 판단하여 경로 생성
    * navmeshagent : 네비게이션 시스템의 이동 가능 경로를 따라가는 역할
    * navmeshobstacle : 내비게이션 시스템의 장애물 오브젝트 자료형
* bounds : collider의 경계 상자 정보
* encapsulation : 객체 지향 프로그래밍의 개념으로, 데이터와, 데이터를 처리하는 메서드를 하나의 단위로 묶어 캡슐화
* offset : 이동량을 나타내는 개념으로, 위치를 상대적으로 이동, 조정할 수 있다
* size : gameobject나 요소의 차원을 나타내는 값
* particlesystemdata : 파티클 시스템 데이터의 개념으로, 파티클 시스템의 속성과 동작을 정의하는 집합
* intersects : 두 개의 객체, 형상이 교차하는지 여부를 확인하는 메서드, 함수
    * bounds.intersects : 두 경계 상자의 교차 여부를 확인
    * collider.intersects : collider클래스 메서드로 collider가 교차하는지의 여부를 확인
    * ray.intersects : ray클래스 메서드로, ray와 형상, 객체가 교차하는지 여부를 확인
    * serializable : attribute중 하나로, 구조체를 직렬화한다, 해당 클래스, 구조체를 노출시키며, 데이터 파일 저장과 네트워크 통신에 사용된다
* textarea : attribute 중 하나로, 문자열 멤버 변수에 대한 다중 줄 편집
* attribute : attribute를 사용시 코드에 대한 추가 정보 제공, 특정 동작을 지정, 클래스, 메서드, 프로퍼티, 필드 등의 멤버에 적용
* tmpro(textmeshpro) : 고성능 텍스트 렌더링 솔루션, Text component보다 많은 기능과 세밀한 제어 제공, 정교한 텍스트 표현
* setactiveobjects : gameobject 배열의 활성화, 비활성화 상태를 일괄적으로 변경하는 메서드
* mathf : 수학 관련 유틸리티 클래스, 여러 수학적인 계산, 값의 변환에 이용된다
* onenable : 스크립트나 오브젝트가 활성화 될때 호출되는 함수
* ondisable : 해당 컴포넌트가 비활성화될 때 호출되어, 해당 컴포넌트가 다시 활성화될 때까지 실행되지 않는다
* setactive : gameobject클래스의 메서드로, 오브젝트의 활성과 비활성화 상태를 변경하는데 사용된다
* unityeditor.editorapplication.exitplaymode : unityeditor에서 현재 playmode를 종료하는데 사용되는 unityeditor의 정적 클래스 editorapplication의 멤버 메서드로, exitplaymode메서드로 실행 중인 플레이 모드를 종료한다
* resources.load : 리소스 폴더 내의 파일을 찾아서 로드하여, 사용할 수 있는 오브젝트나 데이터를 반환한다
* splite : 메서드는 문자열을 지정된 구분자를 기준으로 나누어 배열로 반환한다
* scene : 하나의 독립된 환경이나 장면, 게임 내에서는 특정 레벨, 스테이지, 화면, 메뉴 등을 구성하는 단위로 사용된다
* any state : 다른 모든 상태와 전이가 가능하게하며, 상태 논리를 구성하는데 사용된다.
* conditions : 상태 전이를 제어하는데 사용되는 조건
    * greater : 값의 크기를 비교하여 참과 거짓을 판단한다, 왼쪽의 피연산자의 값이 오른쪽의 피연산자의 값보다 크면 참, 아니면 거짓을 판단하는 역할
    * less : 값의 크기를 비교하여 참과 거짓을 판단한다, 왼쪽의 피연산자 값이 오른쪽의 피연산자의 값보다 작으면 참, 아니면 거짓을 판단하는 역할
    * equals : 왼쪽의 피연산자와 오른쪽의 피연산자의 값이 일치하는지 비교
    * notequal : 왼쪽의 피연산자와 오른쪽의 피연산자의 값이 서로 다른지를 비교
* mask : 이미지나 요소의 특정 부분만을 선택적으로 표시, 나머지 부분을 가린다.
* mask interacion : ui mask 컴포넌트에 사용되는 속성, 마스크된 ui요소와 다른 요소 간의 상호작용 제어
    * visible inside mask : 마스크된 영역 내에만 ui요소가 보인다, 마스크 외부 요소와 상호작용은 차단
    * visible outside mask : 마스크된 영역 내에만 ui요소가 보인다, 필요에 따라 외부 요소와 상호작용여부를 선택한다
    * visible inside mask but not interactable : 마스크된 영역 내에만 ui요소가 보인다, 마스크 내부 요소와의 상호작용 차단, 외부 요소와는 상호작용 가능
    * don't clip : 선택시 해당 ui는 마스크를 적용받지 않고, 화면 전체에 나타나다
* getbuttondown : 버튼이 처음 눌렸을 때만 true를 반환하고, 이후 false를 반환
* getbuttonup : 버튼이 처음 떼어졌을 때만 ture를 반환하고, 이후 false를 반환
* <서로 다른 자료형은 바로 형변환이 이루어지지 않는다>
* updatedialog : 대화 시스템에서 대화 상자를 업데이트하는 기능을 수행하는 메서드나 함수
* sorting layer : 객체들의 렌더링 순서를 관리하는 기능, 객체들을 앞/뒤로 정렬한다
* collsion.contacts : 충돌이 발새한 모든 지점의 정보를 담고있는 배열, contacts는 구조체로 구성되어, 충돌 지점의 위치, 법선 벡터, 접촉면의 마찰력 등의 정보를 저장한다
    * point : 충돌지점의 위치를 나타내는 Vector3 타입 속성
    * normal : 충돌 지점의 법선 벡터를 나타내는 Vector3 타입 속성, 충돌한 두 객체 사이의 충돌 방향과 수직
    * thiscollider : 충돌이 발생한 객체의 콜라이더를 나타내는 collider속성
    * othercollider : 충돌이 발생한 상대 객체의 콜라이더를 나타내는 collider 타입 속성
    * separation : 충돌 지점의 분리 값, 즉 두 객체의 분리 정도를 나타내는 float 타입의 속성
* oncollision : 물리 충돌이 발생할 때 호출되는 함수(2d라면 oncollision(???)2d)
    * oncollisionenter : 물체들이 처음으로 충돌할 때 호출, 충돌할 때 한번만 호출
    * oncollisionstay : 물첻르이 충돌하고 있는 동안 계속해서 호출
    * oncollisionexit : 물체들이 충돌하던 상태에서 분리될 때 호출
* updatedialog : 대화 시스템이나 대화 ui를 업데이트하기 위해 사용되는 함수, 메서드
* <오브젝트의 모듈을 가져오려면, component이후, 해당 모듈에 해당하는 변수를 만들어서 값을 할당해서 사용한다>
* <ani state에 여러개의 animation을 연결하면 우선 순위가 가장 높은 animation만 재생된다, unity의 animation system은 우선순위에 따라서 animation을 재생한다, 하나의 transition에 여러 animation을 연결 시, 마지막에 연결된 animation의 우선순위가 가장 높아지면서, 마지막 animation이 재생된다>
* <다른 오브젝트에서 public 함수를 호출하려면, 해당 오브젝트의 인스턴스 값을 가지고와서 인스턴스 값을 저장한 변수를 통해서 public 함수를 호출해 줄 수 있다>
* <collider를 가진 객체끼리 부딪혔을 때 여러가지 정보를 받아올 수 있다>