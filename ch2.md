#### *객체지향과 인지능력*
>객체란 인간이 부명하게 인지하고 구별할 수 있는 물리적 또는 개념적 경계를 지닌 어떤 것<br>
>ex) 자동차, 컴퓨터, 모니터 .. 오늘의 주문 내역, 어제의 주문내역 등

#### *객체, 그리고 이상한 나라*
- 앨리스 객체
  - 엘리스는 상태를 가지며 상태는 변경 가능함.
  - 앨리스의 상태를 변경시키는 것은 앨리스의 행동임
  - 행동의 결과는 상태에 의존적이며 상태를 이용해 서술할 수 있따.
  - 행동의 순서가 결과에 영향을 미친다.
  - 앨리스는 어떤 상태에 있더라도 유일하게 식별 가능하다.

#### *객체, 그리고 소프트웨어 나라*
> 객체는 구별가능한 식별자, 특징적인 행동, 변경 가능한 상태를 가짐. 
- 상태(state)
- 행동(behavior)
- 식별자(identity)


#### *상태*
##### 왜 상태가 필요한가?
>앨리스의 키와 문의 높이라는 두 가지 상태만 알면 문을 통과하는 행동의 결과를 예측할 수 있다.
>>비행기 탑승 가능 여부는 항공권의 발권 상태를 보고 예측<br>
>>자판기는 현재까지 투입된 금액의 상태를 기억<br>
>>텔레비전 전원이 들어온 상태여야만 채널을 변경가능



#### *상태와 프로퍼티*
- 분명하게 인식할 수 있음에도 객체가 아닌 게 있따.
  - 앨리스의 키, 위치
  - 음료와 케이크의 양
  - 문이 열려있는지 여부
  - 토끼가 달려가는 속도
- 객체의 형태를 표현하는 수단임.

- 프러퍼티 ( 정적, 고정적)
  - 키, 위치 -> 단순값으로 표현됨(속성!), 음료의 양
- 프러퍼티 *값*(동적, 변경됨)

#### *연결(link) : 객체와 객체 사이에 의미있는 연결* 
- 연결되어있어야만 메세지를 보내서 요청할 수 있다.
- 객체는 다른 객체를 참조할 수 있다. (식별자를 알고있다.)
- ??프러퍼티는 속성과 연관관계, 두 가지 종류로 구분된다. 연관관계는 정적인 관계를 의미하며 링크는 연관관계의 인스턴스다.??
- 단순 값인 속성이 있고 링크로 연결된 인스턴스, 즉 2가지라는것...?

#### *객체지향 = 상태 + 상태를 조직하기 위한 행동*
- 객체는 스스로의 행동에 의해서만 상태가 변경된다. (객체의 자율성)
- 다른 객체의 상태를 변경하려면 간접적으로 객체의 상태를 변경해야함.

#### *행동*
##### 상태와 행동
- 객체의 행동은 상태에 영향을 받는다 ?? 행동은 상태에 영향을 준다?
- 객체의 행동은 상태를 변경시킨다.

##### 상태를 이용하면 복잡한 객체의 행동을 쉽게 이해할 수 있다.
>앨리스의 키가 40cm 이하라면 문을 통과할 수 있다.<br>
>문을 통과한 후에 앨리스의 위치는 아름다운 정운으로 바뀌어야 한다.




#### *협력과 행동*
>객체는 다른 객체로부터 메세지를 수신하여 그 요청에 따른 행동을 한다. <br>
>그 과정에서 자신의 상태와 다른 객체의 상태도 변경이 될 수 있음.

##### 행동이란? 
- 외부의 요청 또는 수신된 메세지에 응답하기 위해 동작하고 반응하는 활동.<br>
  - 행동의 결과로 객체는 자신의 상태를 변경하거나 다른 객체에 메세지를 전달할 수 있다.<br>
  - 객체는 행동을 통해 다른 객체와의 협력에 참여하므로 행동은 외부에 가시적이어야 한다.

##### 상태 캡슐화
- 현실 세계와 객체지향 세계의 차이점 : 모든 객체는 자신의 상태를 스스로 관리하는 자율적인 존재임. 
  - 엘리스는 자신이 음료를 마셧다는 메세지를 음료에게 전달할뿐.
- 캡슐화 : 객체는 상태를 캡슐 안에 감춘다. 외부로 노출되는 것은 행동뿐. 외부에서 객체로 접근할 수 있는 것도 행동 뿐.
  - 객체의 자율성을 높임. 
  - 캡슐화는 객체의 자율성을 높이고 협력을 단순, 유연하게 만든다.

##### 식별자
- 모든 객체는 식별자를 가지며 식별자를 이용해 구별할 수 있음.
- 값은 상태만을 이용해 동승성을 판단하기때문에 구분할 필요가 없음.(식별자 필요 x)
  - 동등성 : 상태를 이용해 두 값이 같은지 판단할 수 있는 성질

- 객체는 시간에 따라 변경되는 상태 포함, 행동을 통해 상태 변경, (가변 상태)
  - 타입이 같은 두 객체의 상태가 완전히 똑같아도 두 객체는 독립적인 객체임.
  - 이름이 엘리스가 키가 같은 두 사람이 있다해도 이 둘은 구분된 인격체

- 동일성 : 식별자를 기반으로 객체가 같은지를 판단
  - 객체의 상태는 계쏙 변하기 때문에 식별자를 따로 둔다.
  - 두 객체의 상태가 달라도 식별자가 같다면 동일한 객체
  - 어린시절의 나와 지금의 나.. 상태는 같아도 동일한 객체다
------
- 참조 객체(reference object), 엔티티(entity) : 식별자를 지닌 객체
- 값 객체(value object)  : 식별자를 가지지 않는 값
------
- 객체는 상태를 가지며 상태는 변경 가능하다.
- 객체의 상태를 변경시키는 것은 객체의 행동이다.
  - 행동의 결과는 상태에 의존적이며 상태를 이용해 서술할 수 있다.
  - 행동의 순서가 실행 결과에 영향을 미친다.
- 객체는 어떤 상태에 있더라도 유일하게 시별가능하다.

##### 기계로서의 객체
- (라디오 같은.. 기계를 상상) 명령 버튼, 쿼리 버튼으로 구성된 인터페이스를 통해서만 객체에 접근 가능
  -  상태와 행동이 캡슐화됨

**중요 > 행동이 상태를 결정한다**
- 상태를 먼저 결정하고 나중에 행동을 결정하는 것은 나쁜 설계다
  - 캡슐화가 저해됨. 상태에 초점을 맞출 경우, 상태가 객체 내부로 깔끔하게 캡슐화되지 못하고 공용 인터페이스에 그대로 노출되버릴 확률이 높음
- 상태를 먼저 고려하면 협력을 잘 못하게됨.
- 객체의 재사용성이 저하됨. 다양한 협력을 함으로써 재사용성이 높아짐. 

**협력에 적합한지는 ‘행동’에 의해 결정됨.**

#### *객체지향 설계 방법*
1. 어떤 협력이 필요한지 생각
2. 협력에 참여하는데 필요한 행동을 생각한다.
3. 행동을 수행할 객체를 선택한다.

#### *은유와 객체*
> 두번째 도시 전설 : 객체지향이란 현실 세계의 모방 -> 아님! 이건 오해임

- 의인화 : 현실 객체보다 더 많은 일을 능동적으로 하는 SW의 특징
  - 현실에서의 수동적인 존재가 소프트웨어 안에서는 능동적 객체로 변화함.
   - ex) 현실 속의 전화기는 인간이 행동하기 전에는 역할하지 못함.

- 은유 : 현실의 객체의 개념을 소프트 웨어 객체에 묘사해서 이해를 쉽게한다.

#### *이상한 나라를 창조하라*
>이상한 나라의 앨리스의 등장인물들은 현실세계의 존재와 다르지만 그 현실 존재의 은유적인 의미를 지니고 있음. <br>
>그러면서 능동적인 존재임. (SW객체와 아주 유사함)