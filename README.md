ReactJS로 영화 웹 서비스 만들기 - nomadcoders.co


이하 개발노트

#5 [2021 UPDATE] CREATE REACT APP
#5.0 Introduction
create-react-app을 사용한 react 프로젝트 만들기
빠른 개발환경 구축, 개발서버 접근, 자동 새로고침, 즉각적 CSS 반영 등의 편의

필요 사항
Node.js 설치 (nodejs.org) 
-> console에서 > node -v (버전확인)
-> console에서 > npx (node 확장 모듈 
- 모듈을 로컬에 저장하는대신 최신버전을 임시로 가져와 설치후 삭제)

기존의 react-for-beginners는 삭제한 상태
(현재 디렉토리에 없음)

> npx create-react-app react-for-beginners
react app을 설치한다.

package.json 
script 부분은 미리 만들어진 명령들이다.

> npm start
개발용 서버를 통한 프로젝트 실행

src - 모든 코드가 들어갈곳
index.js - ReactDOM, document.getElementByID 와 같이 
페이지 랜더링을 위한 최상위 component 실행이 정의 되어있다.
rendering 부분과 App component의 jsx를 확인할 수 있다.

index.html - index.js의 실행결과를 body~div#root에서 실행한다.
실제 구동시 보이는 body 이후 3개의 script 구문은 실행시에 자동으로 삽입된다.

실행 화면에 보이는 것과 같이 scr/App.js에서 구문을 수정하면
자동 재랜더링(Auto-reload)되어 바로 화면에 반영되는것을 확인할 수 있다.


index.js에서 필요없는 부분은 모두 정리한다. 
(reder구문의 component들을 삭제)

App.js의 최상위 div를 남겨두고 css들과 모두 삭제한다.

App.test.js, App.css, index.css, logo.svg, reportWebVitals.js, setupTests.js 삭제
(index.js, App.js만 남는다.)

(ReactJS 버전이 달라서 강의와 코드 구성이 다르니 참고.)