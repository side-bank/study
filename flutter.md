코딩셰프 플러터 강좌

https://www.youtube.com/watch?v=AdYRASHRKwE&t=541s

# 순한맛

1. 우리는 왜 플러터를 학습해야 할까요?

* 구글이 가지고 있는 OS
  * 푸시아(Fuchsia) OS
    * 마이크로 커널을 기반으로 하고 있는 OS
  * 안드로이드 OS
  * 크롬 OS

* 커널

  * 운영체제 구동시 하드웨어와 소프트웨어를 연결
  * 마이크로 커널 - 푸시아에서 사용, 구글에서 개발
    * 커널에 최소한의 필수적인 기능만 넣음
  * 단일형 커널 - 안드로이드에서 사용, 오픈소스인 리눅스 커널
    * 커널에 필요한 모든 기술을 커널의 한곳에 모아 놓음
    * 커널의 모든 기능이 한 곳에 모여 있어 수정이나 업데이트가 어렵다. -> 안드로이드 파편화의 원인

* 구글이 푸시아 OS를 만들려는 이유

  * 지르콘은 임베디드 응요프로그램에서 일반적으로 사용되는 소형 시스템용으로 설계된 Little Kernel의 파생물이다.
  * 지르콘은 현대적 전화기와 고속의 프로세서를 갖춘 개인용 컴퓨터를 하고 있다.
  * 음성명령에 중점을 두고 개발됨
  * 안드로이드의 파편화
  * 오라클과의 자바 특허 전쟁

* 플러터(Flutter)

  * 프레임워크
  * 퓨시아 사용자 인터페이스와 어플리케이션을 만들기 위해 사용
  * 플러터 앱 개발을 위한 프로그래밍 언어: 다트(Dart)
  * 크로스 플랫폼 어플리케이션 개발 - 한번의 코딩으로 안드로이드와 iOS 앱을 동시에 만들 수 있다.
  * 인터페이스나 사용자 경험을 하나로 통일
  * 웹앱도 만들 수 있다. - Hummingbird 프로젝트 (매우 초기 단계, 아직 적용하기는 이름...)

* 구글은 왜 플러터를 강력하게 지원하고 있나?

  * 플러터를 사용하면 한번에 안드로이드와 iOS앱을 만들 수 있고, 이를 사용하는 개발자들이 늘어나면 퓨시아 OS를 위한 생태계가 커진다. -> 구글의 노림수

    

1. SDK 설치와 환경변수 설정하기

* Flutter SDK 설치

  * SDK(Software Development Kit): 소스코드의 모음과 유틸리티, 구글이 제공

* 환경변수 설정

  

1. 안드로이드 스튜디오, 비주얼 스튜디오 코드, 에뮬레이터 설치하기

* 안드로이드 스튜디어 / 에뮬레이터 설치

* Visual Studio Code(ide) 설치

  * flutter plugin
  * matirial icon theme

  

1. 플러터 닥터 설정 및 프로젝트 생성하고 에뮬레이터에서 실행해 보기

* Flutter doctor로 실행환경 점검
* Visual Studio Code로 프로젝트 생성 / 에뮬레이터 실행
* Android studio로 프로젝트 생성 / 에뮬레이터 실행



1. 플러터에서 제일 중요하다는 위젯이란 무엇일까요?

* Flutter 상에서의 위젯이란?
  * 위젯: 독립적으로 실행되는 작은 프로그램. 그래픽이나 데이터를 처리하는 함수를 가지고 있음
  * 플러터 상에서 위젯
    * 앱의 UI를 만들고 구성하는 모든 기본 단위 요소
    * +눈에 보이지 않는 요소들까지 위젯
    * **Flutter의 모든 것은 Widget이다**
  * 플러터에서 중요한 3가지 위젯
    * Stateless Widget
      * 스크린상에 존재만 할 뿐 아무것도 하지 않음
      * 어떠한 실시간 데이터도 저장하지 않음
      * 어떤 변화(모양, 상태)를 유발하는 값도 가지지 않음
    * Stateful Widget 
      * 사용자의 인터렉션에 따라 모양이 바뀜
      * 데이터에 따라 모양이 바뀜
    * Inherited Widget
* Stateless widgets vs Stateful widgets
  * Stateful: value값을 지속적으로 추적 보존, **계속 움직임이나 변화가 있는 위젯**
  * Stateless: 이전 상호작용의 어떤 값도 저장하지 않음, **상태가 없는 정적인 위젯**
* Widget tree
  * **위젯은 트리구조로 구성되어 있다** - 부모위젯과 자식 위젯으로 구성
  * 한 위젯 내에 얼마든지 다른 위젯들이 포함될 수 있음 -> html 처럼...
  * Parent widget을 widget Container라고도 함
* 예제 프로젝트 MyApp
  * MyApp - MerterialApp - MyHomePage - **Scaffold** - Image, Button, Text ....
  * Scaffold
    * AppBar - Text
    * Center - Column
      * Image
      * TextField
      * Button



1. 프로젝트 폴더와 기본 코드 이해하기 1, 2, 3
   * Flutter 프로젝트 폴더의 구성
     * 클래스명: MyApp()
     * 함수명: main(), runApp()
   * 코드이 기본내용 이해 / 앱페이지 기본 구성 공식화
   * 첫번째 Flutter 앱 실행



1. 캐릭터 페이지 디자인 1: 위젯정리
2. 캐릭터 페이지 디자인 2: 실전코딩 part1
3. 캐릭터 페이지 디자인 3: 실전코딩 part2 (완결편)



1. 플러터 다트(dart) 핵심 정리: 클래스와 위젯의 정체 1

* 클래스와 위젯

  * 클래스 - 속성, 기능을 정의 => 인스턴스 - 모양, 기능은 완벽하게 동일하지만 각 인스턴스는 구분 가능함
  * 클래스
    * 객체가 가져야 하는 속성과 기능을 정의한 내용을 담고 있는 설계도 역할
  * 객체
    * 클래스가 정의된 후 메모리 상에 할당되었을 때 이를 객체라고 함
  * 인스턴스
    * 클래스를 기반으로 생성됨
    * 클래스의 속성과 기능을 똑같이 가지고 있고, 프로그래밍 상에서 사용되는 대상
  * https://dartpad.dev/

* 예제

  ````dart
  class Person {
    String name;
    int age;
    String sex;
  }
  
  void main() {
    Person p1 = new Person();
    p1.age = 30;
    print(p1.age);
  }
  ````

  

1. 플러터 다트(dart) 핵심 정리: 클래스와 위젯의 정체 2

* 생성자와 관련된 함수의 구조와 기능

* 생성자의 구조와 역할

* 클래스와 위젯의 관계

  

1. 앱바(app bar) 메뉴 아이콘 추가하기

* leading: 아이콘 버튼이나 간단한 위젯을 왼쪽에 배치
* actions: 복수의 아이콘 버튼 등을 오른쪽에 배치할 때
* onPressed: 함수의 형태로 일반 버튼이나 아이콘 버튼을 터치했을 때 일어나는 이벤트 정의



1. Drawer 메뉴 만들기 1, 2



1. 아리송한 BuildContext 이해하기

* widget tree에서 현재 widge의 위치를 알 수 있는 정보
  * build함수는 Scaffold라는 Widget을 리턴하는데, 이때 위젯 트리상에서 어디에 위치하는가에 대한 정보를 가지고 있는 context를 가지고 리턴해 준다.
* 이 빌드 컨텍스트는 stateless위젯이나 state 빌드 메서드에 의해서 리턴 된 위젯의 부모가 된다. ????



1. 스낵바(Snack bar)와 BuildContext
2. 빌더(Builder widget)없이 스낵바(Snack bar) 만들기와 토스트 메시지(Toast message) 구현하기
3. 컨테이너 위젯(Container widget) 되짚어 보기
4. 컬럼 위젯(Column widget)과 로우 위젯(Row widget) 되짚어 보기
5. 네비게이터(Navigator) 이해하기
6. 네비게이터(Navigator)와 pushNamed 메서드 이해하기
7. 콜렉션(Collection)과 제네릭(Generic)
8. 제네릭스(Generics) 보충수업



# 조금 매운 맛

1. Stateful widget part 1
2. Stateful widget part 2
3. 로그인과 주사위 게임 플러터 앱 만들기 part 1
4. 로그인과 주사위 게임 플러트 앱 만들기 part 2