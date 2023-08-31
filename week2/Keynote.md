# Keynote

## JSX란?

JavaScript 안에 HTML과 유사한 마크업을 작성할 수 있게 해주는 JavaScript용 구문 확장자

## React에서 JSX를 사용하는 목적

JSX는 `React.createElement(component, props, ...children)` 를 호출하기 위한 Syntactic sugar다.  
컴포넌트를 작성하는 다른 방법도 있지만 대부분의 React 개발자는 JSX의 간결함을 선호하며  대부분의 코드베이스에서 이를 사용한다.

## Syntactic sugar

프로그래밍 언어 내에서 사물을 더 쉽게 읽거나 표현할 수 있도록 설계된 구문

## React.createElement

createElement를 사용하면 React element를 생성할 수 있다. JSX를 작성하는 대신 사용할 수 있다.

## React Element

React 앱의 가장 작은 단위  
컴포넌트의 구성요소  
화면에 표시할 내용을 기술한다.  

## React StrictMode

내부 컴포넌트 트리에 대한 추가 개발 동작 및 경고를 활성화할 수 있는 모드  
StrictMode를 사용하면 개발 중에 컴포넌트에서 흔히 발생하는 버그를 조기에 발견할 수 있다.

## VDOM(Virtual DOM)이란?

실제 DOM 구조를 반영한 상태로 메모리에 있는 가상의 DOM  

### 선언적 API란?

React에게 원하는 UI의 상태를 알려주면 DOM이 그 상태와 일치하도록 하는 것

### VDOM은 왜 쓸까?

→ fast enough  
→ maintainable  

- 메모리 상에 있고 실제 화면에 그려야 할 필요는 없기 때문에 실제 DOM 보다는 연산 비용이 적다.  
- 한 번의 계산만으로도 바뀐 DOM을 적용할 수 있기 때문에 연산의 횟수는 최소한이 된다.  
- 가상 DOM을 사용함으로써 이 과정을 모두 자동화할 수 있고 개발자는 관리할 포인트를 줄일 수 있다.

**_React의 선언적 API를 가능하게 한다. React에게 원하는 UI의 상태를 알려주면 DOM이 그 상태와 일치하도록 한다._**

### - DOM(The Document Object Model : 문서 객체 모델)이란?

HTML, XML 문서의 각 항목을 계층으로 표현하여 생성, 변형, 삭제할 수 있도록 돕는 인터페이스

### - DOM과 Virtual DOM의 차이

DOM은 브라우저가 웹 페이지의 구조와 콘텐츠를 표현한 것으로 개발자가 JavaScript를 직접 사용하여 페이지와 상호작용하고 페이지를 조작할 수 있도록 한다.  
Virtual DOM은 React와 같은 프레임워크에서 실제 DOM과의 직접적인 상호 작용을 최소화하고 UI 업데이트 프로세스를 최적화하여 성능을 향상시키는 데 사용되는 추상화이다.

## Reconciliation(재조정) 과정은 무엇인가?

UI의 이상적인 또는 "가상"적인 표현을 메모리에 저장하고 ReactDOM과 같은 라이브러리에 의해 "실제" DOM과 동기화하는 과정

## +) DOM 추가 학습

[모던 JavaScript 튜토리얼](https://ko.javascript.info/
)
