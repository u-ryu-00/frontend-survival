# Keynote

## Express 란

Node.js를 위한 빠르고 개방적인 간결한 웹 프레임워크

웹 애플리케이션, API 개발을 위해 설계되었다. Node.js의 사실상의 표준 서버 프레임워크로 불리고 있다. Node.js의 핵심 모듈인 http와 Connect 컴포넌트를 기반으로 한다.

## URL 구조

URL(Uniform Resource Locator) : 웹에서 주어진 고유 리소스 주소  
웹에 게시된 리소스를 검색하기 위해 브라우저에서 사용하는 매커니즘이다.

## REST API

REST 아키텍처 스타일을 따르는 API

## HTTP Method(CRUD)

라이언트와 서버 사이에 이루어지는 요청(Request)과 응답(Response) 데이터를 전송하는 방식

서버에 주어진 리소스에 수행하길 원하는 행동, 서버가 수행해야 할 동작을 지정하는 요청을 보내는 방법이다.

## Fetch API 란

네트워크 통신을 포함한 리소스 취득을 위한 인터페이스를 제공하며, XMLHttpRequest보다 강력하고 유연한 대체제

## Promise

자바스크립트 비동기 처리에 사용되는 객체

주로 서버에서 받아온 데이터를 화면에 표시할 때 사용한다.

### 자바스크립트의 비동기 처리

특정 코드의 실행이 완료될 때까지 기다리지 않고 다음 코드를 먼저 수행하는 자바스크립트의 특성

## ReableStream

 바이트 데이터를 읽을수 있는 스트림을 제공하는 Streams API의 인터페이스

## Unicode

전 세계의 모든 문자를 컴퓨터에서 일관되게 표현하고 다룰 수 있도록 설계된 산업 표준

## CORS란

교차 출처 리소스 공유(Cross-Origin Resource Sharing, CORS)

추가 HTTP 헤더를 사용하여, 한 출처에서 실행 중인 웹 애플리케이션이 다른 출처의 선택한 자원에 접근할 수 있는 권한을 부여하도록 브라우저에 알려주는 체제

## React Hook 이란

함수 컴포넌트에서 React state와 생명주기 기능(lifecycle features)을 “연동(hook into)“할 수 있게 해주는 함수

Hook은 class 안에서는 동작하지 않는다. 대신 class 없이 React를 사용할 수 있게 해주는 것이다.

## Hooks

### - useState

상태 유지 값과 그 값을 갱신하는 함수를 반환한다.

### - useEffect

명령형 또는 어떤 effect를 발생하는 함수를 인자로 받는다.

### - useContext

context 객체(React.createContext에서 반환된 값)을 받아 그 context의 현재 값을 반환한다.

### - useRef

.current 프로퍼티로 전달된 인자(initialValue)로 초기화된 변경 가능한 ref 객체를 반환한다.

### - useLayoutEffect

이 함수의 시그니처는 useEffect와 동일하긴 한데, 모든 DOM 변경 후에 동기적으로 발생한다. 이것은 DOM에서 레이아웃을 읽고 동기적으로 리렌더링하는 경우에 사용하면 된다.

## React StrictMode 란

내부 컴포넌트 트리에 대한 추가 개발 동작 및 경고를 활성화할 수 있는 모드  
StrictMode를 사용하면 개발 중에 컴포넌트에서 흔히 발생하는 버그를 조기에 발견할 수 있다.

## useRef

컴포넌트의 생애주기 전체에 걸쳐서 유지되는 객체. 즉, 컴포넌트가 없어질 때까지 동일한 객체가 유지된다.

객체 자체가 값은 아니고, 값을 참조하기 위한 객체. 즉, 언제든지 값을 변경할 수 있다.

상태(state)가 변경되면 해당 컴포넌트와 하위 컴포넌트를 다시 렌더링하지만, 레퍼런스 객체의 현재 값(current)이 바뀌더라도 렌더링에 영향을 주지 않는다.

## Hook의 규칙

Hook은 그냥 JavaScript 함수이지만, 두 가지 규칙을 준수해야 한다.

- 최상위(at the top level)에서만 Hook을 호출해야 한다. 반복문, 조건문, 중첩된 함수 내에서 Hook을 실행하면 안된다.
- React 함수 컴포넌트 내에서만 Hook을 호출해야 한다. 일반 JavaScript 함수에서는 Hook을 호출해서는 안 된다. (Hook을 호출할 수 있는 곳이 딱 한 군데 더 있다. 바로 직접 작성한 custom Hook 내이다.)

## usehooks-ts

바로 사용할 수 있는 React 훅 라이브러리, 타입스크립트로 작성되었다.

### - useBoolean

참/거짓을 다룰 땐 toggle 같이 의도가 명확한 함수를 쓰는 게 좋다.

### - useEffectOnce

의존성 배열을 빈 배열로 넣어서 한 번만 실행하는 Effect를 잡아줄 때가 많은데, 이걸 쓰면 더 명확히 드러난다.

### - useFetch

정말 간단히 쓸 때 좋음.

### - useInterval

React에서 setInterval 등을 쓸 때는 주의해야 할 부분이 있어서 Custom Hook을 만들어서 해결해야 함.

### - useEventListener

모든 종류의 이벤트를 확인할 수 있음. 특히 dispatchEvent로 전달되는 커스텀 이벤트에 반응하기 좋다. (강력 추천!)

### - useLocalStorage

localStorage와 JSON으로 객체 영속화.  
이벤트를 통해(dispatchEvent + useEventListener) 다른 컴포넌트와 동기화하는 게 매우 중요한 특징.

### - useDarkMode

## swr

데이터 가져오기를 위한 React Hooks

SWR은 먼저 캐시(stale)로부터 데이터를 반환한 후, fetch 요청(revalidate)을 하고, 최종적으로 최신화된 데이터를 가져오는 전략이다.

## react-query

React를 위한 강력하고 성능 좋은 데이터 동기화

"전역 상태"를 건드리지 않고도 React 및 React Native 애플리케이션에서 데이터를 가져오고, 캐시하고, 업데이트할 수 있다.
