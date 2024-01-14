# [시간 경과에 따른 STACK-UP 내역]

| 1.   | [**[240113]** ELECTRON 설치 및 React 프로젝트에 장착 실행 테스트 - 성공](##1.-ELECTRON-설치-및-실행-테스트) |
| ---- | ------------------------------------------------------------ |
| 2.   | to be continued...                                           |



## 1. ELECTRON 설치 및 실행 테스트

ELECTRON 장착을 위해 필요한 플러그 인을 설치, 동시 및 순차 실행을 위해 concurrently 모듈과 wait-on 모듈을 둘 다 설치 해야한다. 

```xml
  "dependencies": {
    "@testing-library/jest-dom": "^5.17.0",
    "@testing-library/react": "^13.4.0",
    "@testing-library/user-event": "^13.5.0",
    "concurrently": "^8.2.2",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-scripts": "5.0.1",
    "wait-on": "^7.2.0",
    "web-vitals": "^2.1.4"
  },
```

더해서 package.json에서 실행 명령어를 추가해야한다. 찾아본 블로그 예시들에서는 Electron 환경만 테스트 하기 위해 npm start의 내부 명령어를 바꾸었지만 난 웹 환경 테스트랑 데스크톱 환경 테스트 따로 놔두는게 마음이 편해서 명령어를 전부 따로 따로 작성하였다. 하지만 일렉트론을 개발 단계에서 테스트 하기 위해서는 web 환경으로 테스트 하고 있는 React를 바라봐야 한다. 

<img src=".\GithubImages\Drawing Logic-27.jpg" alt="Drawing Logic-27" style="zoom: 25%;" align="left" />

설명 잘 못하겠는데 요런 식이다. 여튼 내 코드 확인 바라고, 조만간 블로그에 정리해서 여기에 링크 올리겠다.

<img src=".\GithubImages\logic1.PNG" alt="logic1" style="zoom:60%;" />

성공화면 => Web이 아닌 APP 환경에서 띄웠다. 
